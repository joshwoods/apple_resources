

- Nearby Interaction
- NISessionDelegate
-  sessionSuspensionEnded(\_:) 

Instance Method

# sessionSuspensionEnded(\_:)

Notifies you of the end of a session’s suspension.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+watchOS 7.3+

``` source
optional func sessionSuspensionEnded(_ session: NISession)
```

## Parameters 

`session`  

The session that NI suspended.

## Mentioned in 

Extending advanced direction finding and ranging

## Discussion

NI suspends an interaction session when the user backgrounds the app. NI ends the suspension when the user foregrounds the app again. An app may resume a suspended session only after NI invokes this callback. To resume a session after a suspension ends, call run(_:), passing in your session’s configuration.

Session suspension is a local event. The framework suspends only the user’s session when the user or system event such as a phone call backgrounds the app. However, if the app stays backgrounded for too long during a suspension, NI invalidates the session with session(_:didInvalidateWith:) and the peer user’s session invokes session(_:didRemove:reason:) with `reason` NINearbyObject.RemovalReason.timeout.

## See Also

### Managing interruption

func sessionWasSuspended(NISession)

Notifies you of a suspended session.

