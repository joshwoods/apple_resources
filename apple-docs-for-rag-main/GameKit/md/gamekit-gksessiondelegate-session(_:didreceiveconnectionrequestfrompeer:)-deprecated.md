

- GameKit
- GKSessionDelegate
-  session(\_:didReceiveConnectionRequestFromPeer:) Deprecated

Instance Method

# session(\_:didReceiveConnectionRequestFromPeer:)

Received by the delegate when a remote peer wants to create a connection to the session.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
optional func session(
    _ session: GKSession,
    didReceiveConnectionRequestFromPeer peerID: String
)
```

## Parameters 

`session`  

The session that received the request.

`peerID`  

A string that uniquely identifies the peer.

## Discussion

The delegate should call the session’s acceptConnection(fromPeer:) method if it wants to accept the connection or the denyConnection(fromPeer:) method if it wants to refuse the connection.

Important

If a GKPeerPickerController object is being used to configure the session, the controller handles this message automatically. Your delegate can ignore it if the peer picker dialog is in use. If your application is not using a GKPeerPickerController object to configure the session, your delegate must implement this method as described above.

