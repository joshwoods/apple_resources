

- Nearby Interaction
- NINearbyObject
- NINearbyObject.RemovalReason
-  NINearbyObject.RemovalReason.timeout 

Case

# NINearbyObject.RemovalReason.timeout

NI timed out the session.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+watchOS 7.3+

``` source
case timeout
```

## Discussion

The framework times out a session if the peer user closes the app, or if too much time passes in a suspended state (see sessionWasSuspended(_:)). NI may also time out a session to save device resources.

An app must watch for timed-out peers. If the app wishes to continue interaction with a timed-out peer device, the app must begin a new session.

## See Also

### Reasons

case peerEnded

The peer ended the session.

case peerEnded

The peer ended the session.

