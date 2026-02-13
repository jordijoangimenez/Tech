---
layout: default
title: 5GMSd Features
parent: 5G Media Streaming
has_children: false
nav_order: 1
---

<img src="../../assets/images/Banner_5GMS.png" /> 

{: .warning }
This documentation is currently **under development and subject to change**. It reflects outcomes elaborated by 5G-MAG members. If you are interested in becoming a member of the 5G-MAG and actively participating in shaping this work, please contact the [Project Office](https://www.5g-mag.com/contact)

## Key Features for 5GMSd

The following features are defined for Downlink Media Streaming.

Feature | Description | Procedure | APIs 
--- | --- | --- | ---
Content hosting | 3GPP TS 26.501 4.0.2 | 3GPP TS 26.501 5.4 | 3GPP TS 26.510 + 26.512
Network assistance | 3GPP TS 26.501 4.0.5 | 3GPP TS 26.501 5.9 | 3GPP TS 26.510 + 26.512
Dynamic policies | 3GPP TS 26.501 4.0.6 | 3GPP TS 26.501 5.8 | 3GPP TS 26.510 + 26.512
Consumption reporting | 3GPP TS 26.501 4.0.8 | 3GPP TS 26.501 5.6 | 3GPP TS 26.510 + 26.512
QoE metrics reporting | 3GPP TS 26.501 4.0.9 | 3GPP TS 26.501 5.5 | 3GPP TS 26.510 + 26.512
Edge processing | 3GPP TS 26.501 4.0.10 | 3GPP TS 26.501 8 | 3GPP TS 26.510 + 26.512
eMBMS delivery | 3GPP TS 26.501 4.0.11 | 3GPP TS 26.501 5.10 | 3GPP TS 26.510 + 26.512
Data collection, reporting and exposure | 3GPP TS 26.501 5.11 | 3GPP TS 26.510 + 26.512

## Feature: Content Hosting

{: .referencetools }
Go to the [5G Media Streaming Project](https://hub.5g-mag.com/Getting-Started/pages/5g-media-streaming/)

### Description
The content hosting feature provides a service equivalent to a Content Delivery Network (CDN) deployed inside or outside the Trusted DN.

<img src="./images/5GMS_ContentHosting.png" width="80%">

### Reference points and interactions (according to 3GPP TS 26.510)

Reference Point | Interactions | API Name | Description
--- | --- | --- | ---
M1 | 5.2.2 | [Provisioning Sessions API](https://jdegre.github.io/loader.html?yaml=TS26512_M1_ProvisioningSessions.yaml) | 8.2
M1 | 5.2.3 | [Content protocols discovery API](https://jdegre.github.io/loader.html?yaml=TS26512_M1_ContentProtocolsDiscovery.yaml) | 8.3
M1 | 5.2.4 | [Server Certificates provisioning API](https://jdegre.github.io/loader.html?yaml=TS26512_M1_ServerCertificatesProvisioning.yaml) | 8.4
M1 | 5.2.5 | [Content Preparation Templates provisioning API](https://jdegre.github.io/loader.html?yaml=TS26512_M1_ContentPreparationTemplatesProvisioning.yaml) | 8.5
M1 | 5.2.6 | [Edge Resources provisioning API](https://jdegre.github.io/loader.html?yaml=TS26512_M1_EdgeResourcesProvisioning.yaml) | 8.6
M1 | 5.2.7 | [Policy Templates provisioning API](https://jdegre.github.io/loader.html?yaml=TS26512_M1_PolicyTemplatesProvisioning.yaml) | 8.7
M1 | 5.2.8 | [Content Hosting provisioning API](https://jdegre.github.io/loader.html?yaml=TS26512_M1_ContentHostingProvisioning.yaml) | 8.8
M5 | 5.3.2 | [Service Access Information API](https://jdegre.github.io/loader.html?yaml=TS26512_M5_ServiceAccessInformation.yaml) | 9.2

## Feature: Network Assistance

### Description
The network assistance feature enables the 5GMS Client in the UE to interrogate or manipulate the network Quality of Service for an ongoing media streaming session.

<img src="./images/5GMS_NetworkAssistance.png" width="80%">

### Reference points and interactions (according to 3GPP TS 26.510)

Reference Point | Interactions | API Name | Description
--- | --- | --- | ---
M1 | 5.2.2 | [Provisioning Sessions API](https://jdegre.github.io/loader.html?yaml=TS26512_M1_ProvisioningSessions.yaml) | 8.2
M1 | 5.2.3 | [Content protocols discovery API](https://jdegre.github.io/loader.html?yaml=TS26512_M1_ContentProtocolsDiscovery.yaml) | 8.3
M1 | 5.2.4 | [Server Certificates provisioning API](https://jdegre.github.io/loader.html?yaml=TS26512_M1_ServerCertificatesProvisioning.yaml) | 8.4
M1 | 5.2.5 | [Content Preparation Templates provisioning API](https://jdegre.github.io/loader.html?yaml=TS26512_M1_ContentPreparationTemplatesProvisioning.yaml) | 8.5
M1 | 5.2.6 | [Edge Resources provisioning API](https://jdegre.github.io/loader.html?yaml=TS26512_M1_EdgeResourcesProvisioning.yaml) | 8.6
M1 | 5.2.7 | [Policy Templates provisioning API](https://jdegre.github.io/loader.html?yaml=TS26512_M1_PolicyTemplatesProvisioning.yaml) | 8.7
M1 | 5.2.8 | [Content Hosting provisioning API](https://jdegre.github.io/loader.html?yaml=TS26512_M1_ContentHostingProvisioning.yaml) | 8.8
M5 | 5.3.2 | [Service Access Information API](https://jdegre.github.io/loader.html?yaml=TS26512_M5_ServiceAccessInformation.yaml) | 9.2












### Features: Dynamic Policy instantiation (TS 26.510)

Reference Point | Interactions | API Name | API
--- | --- | --- | ---
M1 | 5.2.2 | Provisioning Sessions API | 8.3
M1 | 5.2.7 | Policy Templates provisioning API | 8.7
M5 | 5.3.2 | Service Access Information API | 9.2
M5 | 5.3.3 | Dynamic Policies API | 9.3

### Features: Network Assistance (TS 26.510)

Reference Point | Interactions | API Name | API
--- | --- | --- | ---
M5 | 5.3.2 | Service Access Information API | 9.2
M5 | 5.3.4 | Network Assistance API | 9.4

### Features: QoE Metrics reporting (TS 26.510)

Reference Point | Interactions | API Name | API
--- | --- | --- | ---
M1 | 5.2.2 | Provisioning Sessions API | 8.3
M1 | 5.2.11 | Metrics Reporting provisioning API | 8.10
M5 | 5.3.2 | Service Access Information API | 9.2
M5 | 5.3.5 | Metrics Reporting API | 9.5

### Features: Consumption reporting (TS 26.510)

Reference Point | Interactions | API Name | API
--- | --- | --- | ---
M1 | 5.2.2 | Provisioning Sessions API | 8.3
M1 | 5.2.12 | Consumption Reporting provisioning API | 8.12
M5 | 5.3.2 | Service Access Information API | 9.2
M5 | 5.3.6| Consumption Reporting API | 9.6

### Features: UE data collection, reporting and exposure (TS 26.510)

Reference Point | Interactions | API Name | API
--- | --- | --- | ---
M1 | 5.2.13 | Event Data Processing provisioning API | 8.13
M5 | 5.3.5 | Metrics Reporting API | 9.5
M5 | 5.3.6 | Consumption Reporting API | 9.6





















## Content Hosting

<img src="./images/5GMS_ContentHosting.png" width="80%">


Reference Point | Interactions | API Name | API
--- | --- | --- | ---
M1 | 5.2.2 | Provisioning Sessions API | 8.2
M1 | 5.2.3 | Content protocols discovery API | 8.3
M1 | 5.2.4 | Server Certificates provisioning API | 8.4
M1 | 5.2.5 | Content Preparation Templates provisioning API | 8.5
M1 | 5.2.6 | Edge Resources provisioning API | 8.6
M1 | 5.2.7 | Policy Templates provisioning API | 8.7
M1 | 5.2.8 | Content Hosting provisioning API | 8.8
M5 | 5.3.2 | Service Access Information API | 9.2

{: .referencetools }
Go to the [5G Media Streaming Project](https://hub.5g-mag.com/Getting-Started/pages/5g-media-streaming/)

### Features: Content Publishing (TS 26.510)

Reference Point | Interactions | API Name | API
--- | --- | --- | ---
M1 | 5.2.2 | Provisioning Sessions API | 8.2
M1 | 5.2.3 | Content protocols discovery API | 8.3
M1 | 5.2.4 | Server Certificates provisioning API | 8.4
M1 | 5.2.5 | Content Preparation Templates provisioning API | 8.5
M1 | 5.2.6 | Edge Resources provisioning API | 8.6
M1 | 5.2.7 | Policy Templates provisioning API | 8.7
M1 | 5.2.9 | Content Publishing provisioning API | 8.9
M5 | 5.3.2 | Service Access Information API | 9.2

### Features: Dynamic Policy instantiation (TS 26.510)

Reference Point | Interactions | API Name | API
--- | --- | --- | ---
M1 | 5.2.2 | Provisioning Sessions API | 8.3
M1 | 5.2.7 | Policy Templates provisioning API | 8.7
M5 | 5.3.2 | Service Access Information API | 9.2
M5 | 5.3.3 | Dynamic Policies API | 9.3

### Features: Network Assistance (TS 26.510)

Reference Point | Interactions | API Name | API
--- | --- | --- | ---
M5 | 5.3.2 | Service Access Information API | 9.2
M5 | 5.3.4 | Network Assistance API | 9.4

### Features: QoE Metrics reporting (TS 26.510)

Reference Point | Interactions | API Name | API
--- | --- | --- | ---
M1 | 5.2.2 | Provisioning Sessions API | 8.3
M1 | 5.2.11 | Metrics Reporting provisioning API | 8.10
M5 | 5.3.2 | Service Access Information API | 9.2
M5 | 5.3.5 | Metrics Reporting API | 9.5

### Features: Consumption reporting (TS 26.510)

Reference Point | Interactions | API Name | API
--- | --- | --- | ---
M1 | 5.2.2 | Provisioning Sessions API | 8.3
M1 | 5.2.12 | Consumption Reporting provisioning API | 8.12
M5 | 5.3.2 | Service Access Information API | 9.2
M5 | 5.3.6| Consumption Reporting API | 9.6

### Features: UE data collection, reporting and exposure (TS 26.510)

Reference Point | Interactions | API Name | API
--- | --- | --- | ---
M1 | 5.2.13 | Event Data Processing provisioning API | 8.13
M5 | 5.3.5 | Metrics Reporting API | 9.5
M5 | 5.3.6 | Consumption Reporting API | 9.6

