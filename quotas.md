---

copyright:
  years: 2018, 2020
lastupdated: "2020-6-29"

keywords: quotas, resources, limits

subcollection: vpc


---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:codeblock: .codeblock}
{:pre: .pre}
{:screen: .screen}
{:tip: .tip}
{:note: .note}
{:download: .download}

# Quotas and service limits
{: #quotas}

This document covers quotas and limits for {{site.data.keyword.vpc_full}} and the resources available within it. 
{:shortdesc}

## Quotas
{: #vpcquotas}

The following tables show the quotas for various VPC resources.

To increase a quota for a particular resource, [contact support](/docs/get-support?topic=get-support-getting-customer-support). 
{:note}

### VPCs
{: #vpc-quotas}

|   Resource     | Quota |
| ------- | ------ |
| Virtual private clouds | 10 per region|    
| Subnets | 15 per VPC |  
| Address prefixes | 15 per VPC |  
{: caption="Table 1. Quotas for the VPC service" caption-side="top"}

### Virtual server instances
{: #vsi-quotas}

|   Resource     | Quota | 
| ------- | ------ | 
| vCPU |  200 per region  |   
| RAM | 1600 GB per region |   
| Floating IP addresses | 20 per zone |   
| SSH keys | 200 per account |   
| GPUs (POWER only) | 16 per region |   
{: caption="Table 2. Quotas for virtual server instances" caption-side="top"}

### Dedicated hosts (Beta)
{: #dedicated-host-quotas}

If you provision dedicated hosts, the vCPU associated with your dedicated hosts counts toward the total vCPU for virtual server instances per region. For more information, see [Virtual server instances](/docs/vpc?topic=vpc-quotas#vsi-quotas). 


### Security groups
{: #security-group-quotas}

|Resource|Quota| 
|--------|-----| 
|Security groups|25 per VPC|  
|Rules|25 per security group|   
|Remote rules|5 per security group|  
|Network interfaces|5 per security group|    
{: caption="Table 3. Quotas for security groups" caption-side="top"}

### Access control lists
{: #acl-quotas}

|Resource|Quota|
|--------|-----| 
|ACLs| 25 per VPC |  
|Inbound rules|25 per ACL |  
|Outbound rules |25 per ACL |  
{: caption="Table 4. Quotas for access control lists" caption-side="top"}

### Block storage volumes
{: #block-storage-quotas}

|Resource|Quota| 
|--------|-----| 
| Boot and secondary volumes | 300 total volumes per account in a region<sup>1</sup> |  
<sup>1</sup> You can request to increase the block storage volume limit by submitting an [IBM Support](/docs/vpc?topic=vpc-getting-help) case.
{: caption="Table 5. Quotas for block storage volumes" caption-side="top"}


### VPNs
{: #vpn-quotas}

|Resource|Quota| 
|--------|-----| 
| VPN gateways| 9 per region, 3 per zone |  
| VPN connections | 10 per VPN gateway |  
| IKE policies | 20 per region |  
| IPSec policies | 20 per region |  
| Peer subnets | 50 across all connections of a VPN gateway, 15 per individual VPN connection |  
| Local subnets | 50 across all connections of a VPN gateway, 15 per individual VPN connection |  
{: caption="Table 6. Quotas for the VPN service" caption-side="top"}

### Load balancers
{: #load-balancer-quotas}


|Resource|Quota| 
|--------|-----|
| Load balancers | 20 per region |  
| Listeners | 10 per load balancer |  
| Pools | 10 per load balancer |  
| Members | 50 per pool | 
{: caption="Table 7. Quotas for load balancers" caption-side="top"}

## Service limits
The following table displays current VPC service limits. Unlike quotas, these limits can't be adjusted.

|Resource|Limit| 
|--------|-----|
| VPCs with classic access | 1 per region|
| Network interfaces | 5 per instance |   
| Public Gateways | 1 per zone per VPC |
| Secondary volumes per instance, attached when creating an instance |  4 secondary volumes |
| Secondary volumes per instance, for existing instances with fewer than 4 cores | 4 secondary volumes |
| Secondary volumes per instance, for existing instances with 4 cores or more | Up to 12 secondary volumes |
| Instance groups for auto scale and more  | 200 per account|
{: caption="Table 8. Limits for VPC resources" caption-side="top"}

