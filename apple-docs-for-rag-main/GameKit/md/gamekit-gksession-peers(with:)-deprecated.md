

- GameKit
- GKSession
-  peers(with:) Deprecated

Instance Method

# peers(with:)

Returns a list of peers in the specified connection state.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–2.0Deprecated

``` source
func peers(with state: GKPeerConnectionState) -> [Any]!
```

Deprecated

No longer supported.

## Parameters 

`state`  

The connection state to search for. See GKPeerConnectionState for possible values.

## Return Value

An array of NSString objects with a peerID string for each peer visible to the session that is currently in the specified connection state. If there are no peers in the specified connection state, this method returns `nil`.

## See Also

### Obtaining Information About Other Peers

func displayName(forPeer: String!) -> String!

Returns a user-readable name for a peer.

Deprecated

