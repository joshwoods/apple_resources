

- GameKit
- GKSession
-  sessionMode Deprecated

Instance Property

# sessionMode

The mode the session uses to find other peers.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–2.0Deprecated

``` source
var sessionMode: GKSessionMode { get }
```

Deprecated

No longer supported.

## Discussion

The session mode changes the behavior of the session when isAvailable is set to true.

- A GKSessionMode.server session advertises itself to local devices using its session ID.

- A GKSessionMode.client session searches for local devices advertising the same session ID. As it discovers available and compatible peers, it calls the delegate’s session(_:peer:didChange:) method.

- A GKSessionMode.peer session both advertises as a server and searches as a client.

## See Also

### Related Documentation

var isAvailable: Bool

A Boolean value that determines whether or not the session wants to connect to new peers.

Deprecated

### Information about the Session

var displayName: String!

The name of the user.

Deprecated

var peerID: String!

A string that identifies your session to other peers.

Deprecated

var sessionID: String!

A string used to filter the list of peers who are allowed to see your session.

Deprecated

