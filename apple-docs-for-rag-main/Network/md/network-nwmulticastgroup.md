

- Network
-  NWMulticastGroup 

Class

# NWMulticastGroup

A descriptor for a group you use to join an IP multicast group on a local network.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
class NWMulticastGroup
```

## Overview

Important

In order to use multicast on iOS, your app will need to have the `com.apple.developer.networking.multicast` entitlement.

## Topics

### Essentials

com.apple.developer.networking.multicast

A Boolean value that indicates whether an app can send or receive IP multicast traffic.

### Defining Multicast Groups

init(for: [NWEndpoint], from: NWEndpoint?, disableUnicast: Bool) throws

Initializes a multicast group with a set of multicast addresses.

### Inspecting Multicast Groups

var members: [NWEndpoint]

The set of IP multicast group addresses that the connection group joins.

let sourceFilter: NWEndpoint?

An optional address endpoint you provide to filter received multicast packets.

let isUnicastDisabled: Bool

A Boolean that specifies whether the connection group rejects unicast traffic.

## Relationships

### Conforms To

- NWGroupDescriptor
- Sendable

## See Also

### Establishing Group Connectivity

init(with: any NWGroupDescriptor, using: NWParameters)

Initializes a new connection group with a group identifier.

protocol NWGroupDescriptor

A protocol that defines a group of endpoints with which you can communicate, such as a multicast group.

func start(queue: DispatchQueue)

Joins the group, registers to receive messages, and sets the queue on you handle group events.

