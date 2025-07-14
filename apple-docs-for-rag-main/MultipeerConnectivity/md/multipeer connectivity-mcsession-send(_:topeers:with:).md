

- Multipeer Connectivity
- MCSession
-  send(\_:toPeers:with:) 

Instance Method

# send(\_:toPeers:with:)

Sends a message to nearby peers.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
func send(
    _ data: Data,
    toPeers peerIDs: [MCPeerID],
    with mode: MCSessionSendDataMode
) throws
```

## Parameters 

`data`  

An instance containing the message to send.

`peerIDs`  

An array of peer ID instances representing the peers that should receive the message.

`mode`  

The transmission mode to use (reliable or unreliable delivery).

## Discussion

This method is asynchronous (nonblocking).

On the recipient device, the session instance calls its delegate instance’s session(_:didReceive:fromPeer:) method with the message after it has been fully received.

## See Also

### Sending Data and Resources

func sendResource(at: URL, withName: String, toPeer: MCPeerID, withCompletionHandler: (((any Error)?) -> Void)?) -> Progress?

Sends the contents of a URL to a peer.

func startStream(withName: String, toPeer: MCPeerID) throws -> OutputStream

Opens a byte stream to a nearby peer.

