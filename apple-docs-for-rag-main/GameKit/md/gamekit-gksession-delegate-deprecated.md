

- GameKit
- GKSession
-  delegate Deprecated

Instance Property

# delegate

The delegate of the session object.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–2.0Deprecated

``` source
weak var delegate: (any GKSessionDelegate)! { get set }
```

Deprecated

No longer supported.

## Discussion

A session’s delegate is responsible for observing changes to other peers running with the same session ID. Your application must set a delegate before making your session known to other peers.

## See Also

### Related Documentation

protocol GKSessionDelegate

An object implements the GKSessionDelegate protocol to control the behavior of a GKSession object. The delegate is called when other visible peers change their state relative to the session. It is also called to determine whether another peer is allowed to connect to the session.

Deprecated

