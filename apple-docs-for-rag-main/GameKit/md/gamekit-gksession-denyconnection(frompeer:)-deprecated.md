

- GameKit
- GKSession
-  denyConnection(fromPeer:) Deprecated

Instance Method

# denyConnection(fromPeer:)

Called by the delegate to reject a connection request received from a remote peer.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func denyConnection(fromPeer peerID: String!)
```

## Parameters 

`peerID`  

The string identifying the peer that initiated the connection to the session.

## Discussion

When your session acts as a server, client peers can discover your session and attempt to connect to it. When a client attempts to connect to the session, the delegate’s session(_:didReceiveConnectionRequestFromPeer:) method is called to decide whether the peer should be connected. Your application calls this method to reject the request or acceptConnection(fromPeer:) to accept it.

## See Also

### Receiving Connections from a Remote Peer

func acceptConnection(fromPeer: String!) throws

Called by the delegate to accept a connection request received from a remote peer.

Deprecated

