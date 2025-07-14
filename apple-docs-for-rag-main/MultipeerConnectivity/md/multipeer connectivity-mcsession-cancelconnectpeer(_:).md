

- Multipeer Connectivity
- MCSession
-  cancelConnectPeer(\_:) 

Instance Method

# cancelConnectPeer(\_:)

Cancels an attempt to connect to a peer.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.0+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
func cancelConnectPeer(_ peerID: MCPeerID)
```

## Parameters 

`peerID`  

The ID of the nearby peer.

## Discussion

Call this method to cancel connections to peers when you are using your own service discovery code instead of an `MCNearbyServiceBrowser` or `MCBrowserViewController` object. It should be called in two situations:

- If your app calls connectPeer(_:withNearbyConnectionData:) and later needs to cancel the connection attempt

- If your app has obtained nearby connection data for a peer but you decide not to connect to the peer

For more information, see the Managing Peers Manually section in the overview of the `MCSession` class reference.

## See Also

### Managing Peers Manually

func connectPeer(MCPeerID, withNearbyConnectionData: Data)

Call this method to connect a peer to the session when using your own service discovery code instead of an `MCNearbyServiceBrowser` or `MCBrowserViewController` object.

var connectedPeers: [MCPeerID]

An array of all peers that are currently connected to this session.

func nearbyConnectionData(forPeer: MCPeerID, withCompletionHandler: (Data?, (any Error)?) -> Void)

Obtains connection data for the specified peer.

