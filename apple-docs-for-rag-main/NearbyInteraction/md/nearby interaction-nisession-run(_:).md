

- Nearby Interaction
- NISession
-  run(\_:) 

Instance Method

# run(\_:)

Starts a session with a nearby peer.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+watchOS 7.3+

``` source
func run(_ configuration: NIConfiguration)
```

## Parameters 

`configuration`  

An object that indicates an interaction session’s features.

## Discussion

This function starts an interaction session between two devices.

Before calling this function, ensure the device supports the features your app requires by first inspecting global deviceCapabilities.

### Restart an Interaction Session

To restart a session as the result of unpausing, call this function as described in pause(). The app calls this function when resuming from session suspension, as described in sessionSuspensionEnded(_:).

Note

A session’s discoveryToken maintains its original value through restarts.

### Prompt for User Approval

The framework prompts for user permission to provide its relative position to nearby peers when it calls this function the first time the app launches. On subsequent calls to this function, the framework consults a preference in Settings that stores the user’s decision. For more information, see Initiating and maintaining a session.

## See Also

### Connecting to A Peer Device

var discoveryToken: NIDiscoveryToken?

A temporary, random identifier for a device.

class NIDiscoveryToken

An object that uniquely identifies a peer that participates in an interaction session.

var configuration: NIConfiguration?

The configuration run by the session.

var delegateQueue: dispatch_queue_t?

The dispatch queue on which the session invokes delegate callbacks.

