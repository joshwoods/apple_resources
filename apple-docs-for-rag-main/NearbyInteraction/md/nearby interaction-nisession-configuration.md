

- Nearby Interaction
- NISession
-  configuration 

Instance Property

# configuration

The configuration run by the session.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+watchOS 7.3+

``` source
@NSCopying
var configuration: NIConfiguration? { get }
```

## Discussion

An app doesn’t set this property. Instead, NI sets its value to reflect the object that the app passed in to run(_:).

## See Also

### Connecting to A Peer Device

var discoveryToken: NIDiscoveryToken?

A temporary, random identifier for a device.

class NIDiscoveryToken

An object that uniquely identifies a peer that participates in an interaction session.

func run(NIConfiguration)

Starts a session with a nearby peer.

var delegateQueue: dispatch_queue_t?

The dispatch queue on which the session invokes delegate callbacks.

