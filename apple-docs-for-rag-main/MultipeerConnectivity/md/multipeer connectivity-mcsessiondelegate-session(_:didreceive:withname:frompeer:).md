

- Multipeer Connectivity
- MCSessionDelegate
-  session(\_:didReceive:withName:fromPeer:) 

Instance Method

# session(\_:didReceive:withName:fromPeer:)

Called when a nearby peer opens a byte stream connection to the local peer.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
func session(
    _ session: MCSession,
    didReceive stream: InputStream,
    withName streamName: String,
    fromPeer peerID: MCPeerID
)
```

**Required**

## Parameters 

`session`  

The session through which the byte stream was opened.

`stream`  

An `NSInputStream` object that represents the local endpoint for the byte stream.

`streamName`  

The name of the stream, as provided by the originator.

`peerID`  

The peer ID of the originator of the stream.

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

func session(MCSession, peer: MCPeerID, didChange: MCSessionState)

Called when the state of a nearby peer changes.

**Required**

func session(MCSession, didReceiveCertificate: [Any]?, fromPeer: MCPeerID, certificateHandler: (Bool) -> Void)

Called to validate the client certificate provided by a peer when the connection is first established.

