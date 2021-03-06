+++
title = "Safety Margin"
pagetitle = "Safety Margin"
description = "Discards those options that have a commission higher than expected."
icon = "fa-money"
weight = 3
alwaysopen = false
+++

Safety Margin is an optional plugin that allows discarding options that have a commission **lower** than expected. The expected commission has to be loaded in safety-margin file, and is the commission over net, in other words, ganancy percentage over option's cost.

## Safety Margin {#safetymargin}

### Goals

The safety margin plugin **discards those options that have a commission lower than expected.** By doing this, only options that have a commission over net, equal or lower than those reported in the file will be returned. Remember that, the commission is the ganancy percentage over option cost.

Sequentially, the rules will be evaluated until a match is found, upon finding it, the process will be stopped and the commission will be evaluated. In the same way, if the rule is not found, the option will be validated.  

The matching process uses **client Tokens** filed, which identify the provided by the client and it is used to filter which business rules can be applied in the request sent.

## Files needed in order to use this plugin

* [**Margin safe file format**](/hotelx/plugins/format-files/safety_margin/) (**Mandatory**)

### Execution example



{

    "plugins": {

        "step": "RESPONSE_OPTION",

        "pluginsType": [

            {

                "type": "POST_STEP"

                "name": "safety_margin"

            }

        ]

    }

}
```
