

- Multipeer Connectivity
- MCSessionDelegate
-  session(\_:didFinishReceivingResourceWithName:fromPeer:at:withError:) 

Instance Method

# session(\_:didFinishReceivingResourceWithName:fromPeer:at:withError:)

Indicates that the local peer finished receiving a resource from a nearby peer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
func session(
    _ session: MCSession,
    didFinishReceivingResourceWithName resourceName: String,
    fromPeer peerID: MCPeerID,
    at localURL: URL?,
    withError error: (any Error)?
)
```

**Required**

## Parameters 

`session`  

The session through which the data was received.

`resourceName`  

The name of the resource, as provided by the sender.

`peerID`  

The peer ID of the sender.

`localURL`  

An `NSURL` object that provides the location of a temporary file containing the received data.

`error`  

An error object indicating what went wrong if the file was not received successfully, or `nil`.

## Discussion

The file referenced by `resourceURL` is a temporary file. Your app must either read the file or make a copy in a permanent location before this delegate method returns.

## See Also

### MCSession Delegate Methods

func session(MCSession, didReceive: Data, fromPeer: MCPeerID)

Indicates that an `NSData` object has been received from a nearby peer.

**Required**

func session(MCSession, didStartReceivingResourceWithName: String, fromPeer: MCPeerID, with: Progress)

Indicates that the local peer began receiving a resource from a nearby peer.

**Required**

func session(MCSession, didReceive: InputStream, withName: String, fromPeer: MCPeerID)

Called when a nearby peer opens a byte stream connection to the local peer.

**Required**

func session(MCSession, peer: MCPeerID, didChange: MCSessionState)

Called when the state of a nearby peer changes.

**Required**

func session(MCSession, didReceiveCertificate: [Any]?, fromPeer: MCPeerID, certificateHandler: (Bool) -> Void)

Called to validate the client certificate provided by a peer when the connection is first established.

