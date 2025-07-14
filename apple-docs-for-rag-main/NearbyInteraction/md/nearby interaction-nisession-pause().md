

- Nearby Interaction
- NISession
-  pause() 

Instance Method

# pause()

Stops sending distance and direction updates to the peer.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+watchOS 7.3+

``` source
func pause()
```

## Discussion

To resume a paused session, the app calls run(_:), passing in the session’s configuration.

If an app pauses the session for too long, the peer receives session(_:didRemove:reason:) callback with the NINearbyObject.RemovalReason.timeout reason.

## See Also

### Managing life cycle

var delegate: (any NISessionDelegate)?

An object that the framework notifies of session events.

func invalidate()

Stops a running session.

