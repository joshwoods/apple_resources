

- GameKit
- GKSession
-  displayName(forPeer:) Deprecated

Instance Method

# displayName(forPeer:)

Returns a user-readable name for a peer.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func displayName(forPeer peerID: String!) -> String!
```

## Parameters 

`peerID`  

A string that uniquely identifies a peer.

## Return Value

The name for the peer, or `nil` if `peerID` is not associated with a visible peer.

## Discussion

The display name is used to populate your user interface with the names of other peers visible to the session.

## See Also

### Related Documentation

var displayName: String!

The name of the user.

Deprecated

### Obtaining Information About Other Peers

func peers(with: GKPeerConnectionState) -> [Any]!

Returns a list of peers in the specified connection state.

Deprecated

