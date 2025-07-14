

- Multipeer Connectivity
- MCNearbyServiceBrowser
-  startBrowsingForPeers() 

Instance Method

# startBrowsingForPeers()

Starts browsing for peers.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
func startBrowsingForPeers()
```

## Discussion

After this method is called (until you call stopBrowsingForPeers()), the framework calls your delegate’s browser(_:foundPeer:withDiscoveryInfo:) and browser(_:lostPeer:) methods as new peers are found and lost.

## See Also

### Browsing for Peers

func stopBrowsingForPeers()

Stops browsing for peers.

