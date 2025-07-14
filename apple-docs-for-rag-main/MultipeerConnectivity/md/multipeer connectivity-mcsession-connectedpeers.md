

- Multipeer Connectivity
- MCSession
-  connectedPeers 

Instance Property

# connectedPeers

An array of all peers that are currently connected to this session.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
var connectedPeers: [MCPeerID] { get }
```

## See Also

### Managing Peers Manually

func connectPeer(MCPeerID, withNearbyConnectionData: Data)

Call this method to connect a peer to the session when using your own service discovery code instead of an `MCNearbyServiceBrowser` or `MCBrowserViewController` object.

func cancelConnectPeer(MCPeerID)

Cancels an attempt to connect to a peer.

func nearbyConnectionData(forPeer: MCPeerID, withCompletionHandler: (Data?, (any Error)?) -> Void)

Obtains connection data for the specified peer.

