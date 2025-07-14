

- Nearby Interaction
- NISessionDelegate
-  sessionWasSuspended(\_:) 

Instance Method

# sessionWasSuspended(\_:)

Notifies you of a suspended session.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+watchOS 7.3+

``` source
optional func sessionWasSuspended(_ session: NISession)
```

## Parameters 

`session`  

The session that NI suspended.

## Mentioned in 

Initiating and maintaining a session

## Discussion

When NI invokes this callback, the session suspends and doesn’t receive session(_:didUpdate:) callbacks. NI suspends a session when the user backgrounds the app. If the user reactivates the app before NI times out the session, NI calls sessionSuspensionEnded(_:). A suspended session won’t resume on its own. To resume the session, call run(_:) again, passing in your session’s configuration.

If the app stays backgrounded for too long during a suspension, NI invalidates the session (see session(_:didInvalidateWith:)) and the peer user’s session invokes session(_:didRemove:reason:) with `reason` NINearbyObject.RemovalReason.timeout.

Additionally, the system may suspend a session for internal reasons.

## See Also

### Managing interruption

func sessionSuspensionEnded(NISession)

Notifies you of the end of a session’s suspension.

