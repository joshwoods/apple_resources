

- Nearby Interaction
- NISession
-  delegateQueue 

Instance Property

# delegateQueue

The dispatch queue on which the session invokes delegate callbacks.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+watchOS 7.3+

``` source
var delegateQueue: dispatch_queue_t? { get set }
```

## Discussion

By default, NI invokes delegate callbacks on main.

## See Also

### Connecting to A Peer Device

var discoveryToken: NIDiscoveryToken?

A temporary, random identifier for a device.

class NIDiscoveryToken

An object that uniquely identifies a peer that participates in an interaction session.

func run(NIConfiguration)

Starts a session with a nearby peer.

var configuration: NIConfiguration?

The configuration run by the session.

