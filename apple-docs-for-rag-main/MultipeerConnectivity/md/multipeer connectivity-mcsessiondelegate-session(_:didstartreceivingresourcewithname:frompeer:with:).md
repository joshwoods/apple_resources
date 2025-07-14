

- Multipeer Connectivity
- MCSessionDelegate
-  session(\_:didStartReceivingResourceWithName:fromPeer:with:) 

Instance Method

# session(\_:didStartReceivingResourceWithName:fromPeer:with:)

Indicates that the local peer began receiving a resource from a nearby peer.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
func session(
    _ session: MCSession,
    didStartReceivingResourceWithName resourceName: String,
    fromPeer peerID: MCPeerID,
    with progress: Progress
)
```

**Required**

## Parameters 

`session`  

The session that started receiving the resource.

`resourceName`  

The name of the resource, as provided by the sender.

`peerID`  

The sender’s peer ID.

`progress`  

An `NSProgress` object that can be used to cancel the transfer or queried to determine how far the transfer has progressed.

## See Also

### MCSession Delegate Methods

func session(MCSession, didReceive: Data, fromPeer: MCPeerID)

Indicates that an `NSData` object has been received from a nearby peer.

**Required**

func session(MCSession, didFinishReceivingResourceWithName: String, fromPeer: MCPeerID, at: URL?, withError: (any Error)?)

Indicates that the local peer finished receiving a resource from a nearby peer.

**Required**

func session(MCSession, didReceive: InputStream, withName: String, fromPeer: MCPeerID)

Called when a nearby peer opens a byte stream connection to the local peer.

**Required**

func session(MCSession, peer: MCPeerID, didChange: MCSessionState)

Called when the state of a nearby peer changes.

**Required**

func session(MCSession, didReceiveCertificate: [Any]?, fromPeer: MCPeerID, certificateHandler: (Bool) -> Void)

Called to validate the client certificate provided by a peer when the connection is first established.

