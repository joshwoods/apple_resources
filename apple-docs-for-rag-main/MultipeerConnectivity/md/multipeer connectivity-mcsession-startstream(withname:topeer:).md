

- Multipeer Connectivity
- MCSession
-  startStream(withName:toPeer:) 

Instance Method

# startStream(withName:toPeer:)

Opens a byte stream to a nearby peer.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
func startStream(
    withName streamName: String,
    toPeer peerID: MCPeerID
) throws -> OutputStream
```

## Parameters 

`streamName`  

A name for the stream. This name is provided to the nearby peer.

`peerID`  

The ID of the nearby peer.

## Return Value

In Swift, an output stream instance. In Objective-C, an output stream object upon success or `nil` if a stream could not be established.

## Discussion

This method is nonblocking.

For more information about performing networking with input and output streams, read Networking Programming Topics.

## See Also

### Sending Data and Resources

func send(Data, toPeers: [MCPeerID], with: MCSessionSendDataMode) throws

Sends a message to nearby peers.

func sendResource(at: URL, withName: String, toPeer: MCPeerID, withCompletionHandler: (((any Error)?) -> Void)?) -> Progress?

Sends the contents of a URL to a peer.

