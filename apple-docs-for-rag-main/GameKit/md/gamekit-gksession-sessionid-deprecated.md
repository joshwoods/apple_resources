

- GameKit
- GKSession
-  sessionID Deprecated

Instance Property

# sessionID

A string used to filter the list of peers who are allowed to see your session.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
var sessionID: String! { get }
```

## Discussion

The session ID is used by sessions configured as servers to advertise itself to other peers and by sessions configured as clients to search for compatible servers. The session ID should be the short name of an approved Bonjour service type.

## See Also

### Information about the Session

var displayName: String!

The name of the user.

Deprecated

var peerID: String!

A string that identifies your session to other peers.

Deprecated

var sessionMode: GKSessionMode

The mode the session uses to find other peers.

Deprecated

