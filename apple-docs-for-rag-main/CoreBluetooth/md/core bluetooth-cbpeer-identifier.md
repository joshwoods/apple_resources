

- Core Bluetooth
- CBPeer
-  identifier 

Instance Property

# identifier

The UUID associated with the peer.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.13+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var identifier: UUID { get }
```

## Discussion

The value of this property represents the unique identifier of the peer. The first time a local manager encounters a peer, the system assigns the peer a UUID, represented by a new UUID object. Peers use UUID instances to identify themselves, instead of by the CBUUID objects that identify a peripheral’s services, characteristics, and descriptors.

For more information, see Core Bluetooth Programming Guide.

