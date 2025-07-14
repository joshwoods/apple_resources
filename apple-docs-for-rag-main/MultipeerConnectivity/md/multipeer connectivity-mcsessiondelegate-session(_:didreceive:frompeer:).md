

- Multipeer Connectivity
- MCSessionDelegate
-  session(\_:didReceive:fromPeer:) 

Instance Method

# session(\_:didReceive:fromPeer:)

Indicates that an `NSData` object has been received from a nearby peer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
func session(
    _ session: MCSession,
    didReceive data: Data,
    fromPeer peerID: MCPeerID
)
```

**Required**

## Parameters 

`session`  

The session through which the data was received.

`data`  

An object containing the received data.

`peerID`  

The peer ID of the sender.

## See Also

### MCSession Delegate Methods

func session(MCSession, didStartReceivingResourceWithName: String, fromPeer: MCPeerID, with: Progress)

Indicates that the local peer began receiving a resource from a nearby peer.

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

