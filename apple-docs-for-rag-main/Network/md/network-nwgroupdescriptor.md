

- Network
-  NWGroupDescriptor 

Protocol

# NWGroupDescriptor

A protocol that defines a group of endpoints with which you can communicate, such as a multicast group.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
protocol NWGroupDescriptor : AnyObject, Sendable
```

## Topics

### Inspecting Groups

var members: [NWEndpoint]

The set of endpoints that define the connection group.

**Required**

## Relationships

### Inherits From

- Sendable

### Conforming Types

- NWMulticastGroup
- NWMultiplexGroup

## See Also

### Establishing Group Connectivity

init(with: any NWGroupDescriptor, using: NWParameters)

Initializes a new connection group with a group identifier.

class NWMulticastGroup

A descriptor for a group you use to join an IP multicast group on a local network.

func start(queue: DispatchQueue)

Joins the group, registers to receive messages, and sets the queue on you handle group events.

