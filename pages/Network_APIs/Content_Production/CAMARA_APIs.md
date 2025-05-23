---
layout: default
title: CAMARA APIs
parent: Content Production & Contribution
grand_parent: Network APIs
nav_order: 2
has_children: false
---

{: .warning }
This documentation is currently **under development and subject to change**. It reflects outcomes elaborated by 5G-MAG members as part of **WI: Network Exposure and APIs Supporting Media Services and Applications**
We welcome and encourage contributions from the broader community. If you are interested in becoming a member of the 5G-MAG and actively participating in shaping this work, please contact the [Project Office](https://www.5g-mag.com/contact)

# Requirements coverage by CAMARA APIs

## Quality of Service

 Requirement | CAMARA APIs  
 -- | --
Ability to apply different QoS profiles to individual data flows coming from the same production device node | 
Ability to separate media/data flows coming from the same production device node | 
Delivery to endpoint (Application Media Server) may be identified by security/protocol/IP/port | 
Ability to configure new or re-configure existing QoS profiles to be selected during runtime  | 
Ability to select at runtime a QoS profile for a media flow | 
Ability to receive ACK (success/fail) | 

## Information monitoring, logging and/or Network assistance

 Requirement | CAMARA APIs  
 -- | --
Ability to receive real-time information from the network | 
Ability to receive information from the network during runtime for troubleshooting | 
Ability to receive information from the network after the session (logging information) for post-processing | 

## Time Synchronization

 Requirement | CAMARA APIs  
 -- | --
Ability to enable distribution of timing information | 

# CAMARA APIs within the scope of Content Production & Contribution

## General information

- CAMARA Repositories in GitHub: [Link](https://github.com/orgs/camaraproject/repositories?q=sort%3Aname-asc)
- API Backlog: [Link](https://github.com/camaraproject/WorkingGroups/blob/main/APIBacklog/documentation/APIbacklog.md)
- Proposed new APIs: [Link](https://github.com/camaraproject/WorkingGroups/pulls)

## List of relevant APIs

### [ConnectivityInsights](https://github.com/camaraproject/ConnectivityInsights)

#### Scope
- Service APIs for “Connectivity Insights” (see APIBacklog)
- It provides the customer with the ability to:
  - define intents in the form of policy thresholds for QoS metrics against the device and the application service. The API service will alert the consumers if and when the policy has breached.
  - NOTE: The scope of this API family should be limited (at least at a first stage) to 4G and 5G.

### [DeviceIdentifier](https://github.com/camaraproject/DeviceIdentifier)

#### Scope
- Service APIs for “Device Identifier API” (see API Backlog)
- It provides the customer with the ability to:
  - Retrieve the current identity (IMEI) of the mobile device being used by a given mobile subscriber
  - Retrieve the type (manufacturer and model) of the mobile device being used by a given mobile subscriber

### [DeviceLocation](https://github.com/camaraproject/DeviceLocation)

#### Scope
- Service APIs for “Device Location” (see APIBacklog)
- It provides the customer with the ability to:
  - verify the location of a device (location-verification).
  - retrieve the location of a device (location-retrieval).
  - subscribe and receive notifications about a device entering or leaving certain location (geofencing-subscriptions).
  - NOTE: The scope of this API family should be limited (at least at a first stage) to 4G and 5G.

### [DeviceStatus](https://github.com/camaraproject/DeviceStatus)

#### Scope
- Service APIs for “Device Status” (see APIBacklog)
- It provides the API consumer with the ability to:
  - check if a device is reachable or is not connected to the network
  - check if a device is roaming, and in which country
  - receive notifications if the connectivity or roaming status of the device changes

### [NetworkSliceBooking](https://github.com/camaraproject/NetworkSliceBooking)

#### Scope
- Service APIs for “Network Slice Booking” (see APIBacklog.md)
- It provides the customer with the ability to:
  - reserve, dynamically provisioning, query, dynamically delete a slice with customized SLA assurance capabilities, customized service duration, expected slice covered locations.

### [QualityOnDemand](https://github.com/camaraproject/QualityOnDemand)

#### Scope
- Service APIs for “Quality on Demand” (see APIBacklog.md)
- It provides the API consumer with the ability to:
  - set quality for a flow within an access network connections (e.g. mobile device connection or fixed access between a home gateway and the service providers gateway router)
    - Session mode, for a specific duration
    - Provision mode, indefinitely for each time the device connects to the same access network
  - get notification if the network cannot fulfill
