

- Multipeer Connectivity
- MCSession
-  connectPeer(\_:withNearbyConnectionData:) 

Instance Method

# connectPeer(\_:withNearbyConnectionData:)

Call this method to connect a peer to the session when using your own service discovery code instead of an `MCNearbyServiceBrowser` or `MCBrowserViewController` object.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.0+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
func connectPeer(
    _ peerID: MCPeerID,
    withNearbyConnectionData data: Data
)
```

## Parameters 

`peerID`  

The peer ID object obtained from the nearby peer.

`data`  

The connection data object obtained from the nearby peer.

## Discussion

Call this method to connect to peers when you are using your own service discovery code instead of an `MCNearbyServiceBrowser` or `MCBrowserViewController` object. For more information, see the Managing Peers Manually section in the overview of the `MCSession` class reference.

## See Also

### Managing Peers Manually

func cancelConnectPeer(MCPeerID)

Cancels an attempt to connect to a peer.

var connectedPeers: [MCPeerID]

An array of all peers that are currently connected to this session.

func nearbyConnectionData(forPeer: MCPeerID, withCompletionHandler: (Data?, (any Error)?) -> Void)

Obtains connection data for the specified peer.

