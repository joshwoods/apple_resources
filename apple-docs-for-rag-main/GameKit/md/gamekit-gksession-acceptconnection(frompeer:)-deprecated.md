

- GameKit
- GKSession
-  acceptConnection(fromPeer:) Deprecated

Instance Method

# acceptConnection(fromPeer:)

Called by the delegate to accept a connection request received from a remote peer.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
func acceptConnection(fromPeer peerID: String!) throws
```

## Parameters 

`peerID`  

The string identifying the peer that initiated the connection to the session.

## Discussion

When your session acts as a server, client peers can discover your session and attempt to connect to it. When a client attempts to connect to the session, the delegate’s session(_:didReceiveConnectionRequestFromPeer:) method is called to decide whether the peer should be connected. Your application calls this method to accept the request, or denyConnection(fromPeer:) to reject it.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Receiving Connections from a Remote Peer

func denyConnection(fromPeer: String!)

Called by the delegate to reject a connection request received from a remote peer.

Deprecated

