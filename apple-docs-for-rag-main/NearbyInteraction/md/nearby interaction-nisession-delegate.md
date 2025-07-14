

- Nearby Interaction
- NISession
-  delegate 

Instance Property

# delegate

An object that the framework notifies of session events.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+watchOS 7.3+

``` source
weak var delegate: (any NISessionDelegate)? { get set }
```

## Discussion

An app must set a delegate to receive the peer’s distance and direction information through session(_:didUpdate:). The session(_:didInvalidateWith:) and session(_:didRemove:reason:) callbacks notify you when the session invalidated or removed a peer. The system may suspend an interaction session for various reasons (see sessionWasSuspended(_:)), such as when the peer backgrounds the app.

## See Also

### Managing life cycle

func pause()

Stops sending distance and direction updates to the peer.

func invalidate()

Stops a running session.

