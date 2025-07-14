

- Network
- NWConnectionGroup
-  start(queue:) 

Instance Method

# start(queue:)

Joins the group, registers to receive messages, and sets the queue on you handle group events.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
final func start(queue: DispatchQueue)
```

## See Also

### Establishing Group Connectivity

init(with: any NWGroupDescriptor, using: NWParameters)

Initializes a new connection group with a group identifier.

class NWMulticastGroup

A descriptor for a group you use to join an IP multicast group on a local network.

protocol NWGroupDescriptor

A protocol that defines a group of endpoints with which you can communicate, such as a multicast group.

