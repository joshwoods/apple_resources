

- Nearby Interaction
- NISession
-  invalidate() 

Instance Method

# invalidate()

Stops a running session.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+watchOS 7.3+

``` source
func invalidate()
```

## Discussion

When an app calls this function, NI invokes session(_:didRemove:reason:) on the peer’s side and passes in the `reason` NINearbyObject.RemovalReason.peerEnded. The app can’t restart invalid sessions.

## See Also

### Managing life cycle

var delegate: (any NISessionDelegate)?

An object that the framework notifies of session events.

func pause()

Stops sending distance and direction updates to the peer.

