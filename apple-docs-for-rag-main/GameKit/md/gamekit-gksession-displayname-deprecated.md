

- GameKit
- GKSession
-  displayName Deprecated

Instance Property

# displayName

The name of the user.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
var displayName: String! { get }
```

## Discussion

The display name is transmitted to visible peers so that they can present a human-readable name for your session.

## See Also

### Related Documentation

func displayName(forPeer: String!) -> String!

Returns a user-readable name for a peer.

Deprecated

### Information about the Session

var peerID: String!

A string that identifies your session to other peers.

Deprecated

var sessionID: String!

A string used to filter the list of peers who are allowed to see your session.

Deprecated

var sessionMode: GKSessionMode

The mode the session uses to find other peers.

Deprecated

