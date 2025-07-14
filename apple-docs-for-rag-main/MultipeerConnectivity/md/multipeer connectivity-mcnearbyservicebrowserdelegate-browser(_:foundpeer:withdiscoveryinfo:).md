

- Multipeer Connectivity
- MCNearbyServiceBrowserDelegate
-  browser(\_:foundPeer:withDiscoveryInfo:) 

Instance Method

# browser(\_:foundPeer:withDiscoveryInfo:)

Called when a nearby peer is found.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
func browser(
    _ browser: MCNearbyServiceBrowser,
    foundPeer peerID: MCPeerID,
    withDiscoveryInfo info: [String : String]?
)
```

**Required**

## Parameters 

`browser`  

The browser object that found the nearby peer.

`peerID`  

The unique ID of the peer that was found.

`info`  

The info dictionary advertised by the discovered peer. For more information on the contents of this dictionary, see the documentation for init(peer:discoveryInfo:serviceType:) in MCNearbyServiceAdvertiser.

## Discussion

The peer ID provided to this delegate method can be used to invite the nearby peer to join a session.

## See Also

### Peer Discovery Delegate Methods

func browser(MCNearbyServiceBrowser, lostPeer: MCPeerID)

Called when a nearby peer is lost.

**Required**

