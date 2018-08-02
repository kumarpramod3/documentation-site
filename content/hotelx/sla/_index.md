+++
title = "Service Level Agreements"
pagetitle = "Service Level Agreements for HotelX"
description = "Service Level Agreements for HotelX"
svgicon="/images/sla.svg"
icon="fa-sla"
isDirectory = false
weight = 6
alwaysopen = false
+++

The following are the Service Level Agreements for HotelX

# SLA HotelX

During the Term of the TravelgateX License Agreement (as applicable, the "Agreement"), the Covered Service will provide a Monthly Uptime Percentage to Customer of at least [99.9]% (the “Service Level Objective ” or “SLO”). If TravelgateX does not meet the SLO, and if Customer meets its obligations under this SLA, Customer will be eligible to receive the Financial Credits agreed. This SLA states Customer’s sole and exclusive remedy for any failure by TravelgateX to meet the SLO.

## Definitions

The following definitions apply to the SLA:

* “**Covered Service**” means:

	* Instances hosted as part of the TravelgateX Compute Engine Service.
	* Load balancing as part of the TravelgateX Compute Engine Service.

* “**Downtime**” means:

	* For Instances: Loss of external connectivity or persistent disk access for all running Instances, when Instances are placed across two or more Zones in the same Region.
	* For load balancing: Loss of external connectivity (via the external IP addresses associated with load balancing forwarding rules with all Healthy Backend Instances) due to the failure of TravelgateX’s systems.
	* Downtime does not include loss of external connectivity as a result of the TravelgateX managed VPN service failing to serve traffic directed to VPN tunnels under that service. That sort of downtime is addressed exclusively in the VPN SLA.

* “**Downtime Period**” means a period of one or more consecutive minutes of Downtime. Partial minutes or Intermittent Downtime for a period of less than one minute will not be counted towards any Downtime Periods.

* “**Degradation**” means a quality of service under expected SLO

* “**Degradation percentage**” means the following:

Monthly Uptime Percentage | Percentage of monthly bill for the respective Covered Service in which did not meet SLO that will be credited to future monthly bills of Customer
------------------------- | -------------------------
99.00% - < 99.99% | 10%
95.00% - < 99.00% | 25%
< 95.00% | 50%

* “**Monthly Uptime Percentage**” means total number of minutes in a month, minus the number of minutes of Downtime suffered from all Downtime Periods in a month, divided by the total number of minutes in a month.

* “**Healthy Backend Instances**” means Instances that are responding affirmatively to load balancing health checks.

## SLA Exclusions

The SLA does not apply to any: (a) features designated Alpha or Beta (unless otherwise set forth in the associated Documentation), (b) features excluded from the SLA (in the associated Documentation), or (c) errors: (i) caused by factors outside of TravelgateX’s reasonable control; (ii) that resulted from Customer’s software or hardware or third party software or hardware, or both; (iii) that resulted from abuses or other behaviors that violate the Agreement; or (iv) that resulted from quotas applied by the system and/or listed in the Admin Console.

