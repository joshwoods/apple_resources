

- Multipeer Connectivity
- MCSessionDelegate
-  session(\_:peer:didChange:) 

Instance Method

# session(\_:peer:didChange:)

Called when the state of a nearby peer changes.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
func session(
    _ session: MCSession,
    peer peerID: MCPeerID,
    didChange state: MCSessionState
)
```

**Required**

## Parameters 

`session`  

The session that manages the nearby peer whose state changed.

`peerID`  

The ID of the nearby peer whose state changed.

`state`  

The new state of the nearby peer.

## Discussion

This delegate method is called with the following state values when the nearby peer’s state changes:

- MCSessionState.connected—the nearby peer accepted the invitation and is now connected to the session.

- MCSessionState.notConnected—the nearby peer declined the invitation, the connection could not be established, or a previously connected peer is no longer connected.

## See Also

### MCSession Delegate Methods

func session(MCSession, didReceive: Data, fromPeer: MCPeerID)

Indicates that an `NSData` object has been received from a nearby peer.

**Required**

func session(MCSession, didStartReceivingResourceWithName: String, fromPeer: MCPeerID, with: Progress)

Indicates that the local peer began receiving a resource from a nearby peer.

**Required**

func session(MCSession, didFinishReceivingResourceWithName: String, fromPeer: MCPeerID, at: URL?, withError: (any Error)?)

Indicates that the local peer finished receiving a resource from a nearby peer.

**Required**

func session(MCSession, didReceive: InputStream, withName: String, fromPeer: MCPeerID)

Called when a nearby peer opens a byte stream connection to the local peer.

**Required**

func session(MCSession, didReceiveCertificate: [Any]?, fromPeer: MCPeerID, certificateHandler: (Bool) -> Void)

Called to validate the client certificate provided by a peer when the connection is first established.

