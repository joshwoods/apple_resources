

- Multipeer Connectivity
- MCBrowserViewControllerDelegate
-  browserViewController(\_:shouldPresentNearbyPeer:withDiscoveryInfo:) 

Instance Method

# browserViewController(\_:shouldPresentNearbyPeer:withDiscoveryInfo:)

Called when a new peer is discovered to decide whether to show it in the user interface.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
optional func browserViewController(
    _ browserViewController: MCBrowserViewController,
    shouldPresentNearbyPeer peerID: MCPeerID,
    withDiscoveryInfo info: [String : String]?
) -> Bool
```

## Parameters 

`browserViewController`  

The browser view controller object that discovered the new peer.

`peerID`  

The unique ID of the nearby peer.

`info`  

The info dictionary advertised by the discovered peer. For more information on the contents of this dictionary, see the documentation for init(peer:discoveryInfo:serviceType:) in MCNearbyServiceAdvertiser.

## Return Value

This delegate method should return true if the newly discovered peer should be shown in the user interface, or false otherwise.

## Discussion

If this method is not provided, all peers are shown.

