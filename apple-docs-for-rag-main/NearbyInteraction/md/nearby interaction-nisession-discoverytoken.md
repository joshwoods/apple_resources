

- Nearby Interaction
- NISession
-  discoveryToken 

Instance Property

# discoveryToken

A temporary, random identifier for a device.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+watchOS 7.3+

``` source
@NSCopying
var discoveryToken: NIDiscoveryToken? { get }
```

## Mentioned in 

Initiating and maintaining a session

Discovering peers with Multipeer Connectivity

## Discussion

NI sets this property when an app initializes a session. The value of discoveryToken is unique to the session and identifies the device that created the session.

To begin a session, an app shares this object with a nearby peer using a network technology that both devices agree to. For an example that shares discovery tokens using Multipeer Connectivity, see Implementing Interactions Between Users in Close Proximity.

## See Also

### Connecting to A Peer Device

class NIDiscoveryToken

An object that uniquely identifies a peer that participates in an interaction session.

func run(NIConfiguration)

Starts a session with a nearby peer.

var configuration: NIConfiguration?

The configuration run by the session.

var delegateQueue: dispatch_queue_t?

The dispatch queue on which the session invokes delegate callbacks.

