---
layout: default
title: Requirements by Network API Initiatives
parent: Content Production & Contribution
grand_parent: Network APIs
nav_order: 3
has_children: false
---

{: .warning }
This documentation is currently **under development and subject to change**. It reflects outcomes elaborated by 5G-MAG members as part of **WI: Network Exposure and APIs Supporting Media Services and Applications**
We welcome and encourage contributions from the broader community. If you are interested in becoming a member of the 5G-MAG and actively participating in shaping this work, please contact the [Project Office](https://www.5g-mag.com/contact)

# Requirements coverage by Network API inititives

## CAMARA APIs

### Media delivery with Quality of Service (QoS)

 Requirement | API  
 -- | --
Ability to apply different QoS profiles to individual data flows coming from the same production device node | 
Ability to separate media/data flows coming from the same production device node | 
Delivery to endpoint (Application Media Server) may be identified by security/protocol/IP/port | 
Ability to configure new or re-configure existing QoS profiles to be selected during runtime  | 
Ability to select at runtime a QoS profile for a media flow | 
Ability to receive ACK (success/fail) | 

### Information monitoring, logging and/or Network assistance

 Requirement | API
 -- | --
Ability to receive real-time information from the network | 
Ability to receive information from the network during runtime for troubleshooting | 
Ability to receive information from the network after the session (logging information) for post-processing | 

### Time Synchronization

 Requirement | API  
 -- | --
Ability to enable distribution of timing information | 

### Voice service for Intercom

 Requirement | API 
 -- | --
Ability to establish a voice service across the intercom devices deployed at the production location or between the production center and the production location | 

## Considerations for API selection

### Identification of devices
  - Devices should be uniquely identifiable during operation
  - Devices should be dynamically added or deleted during operation and attachable to given network capabilities
  - Each device should only access the network capabilities which have been assigned during booking.

### Device on-boarding and API consumer on-boarding
- TBD How to obtain credentials

### Discovery of network capabilities
- TBD How to discover network capabilities
