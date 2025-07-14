

- Multipeer Connectivity
- MCNearbyServiceBrowserDelegate
-  browser(\_:didNotStartBrowsingForPeers:) 

Instance Method

# browser(\_:didNotStartBrowsingForPeers:)

Called when a browser failed to start browsing for peers.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
optional func browser(
    _ browser: MCNearbyServiceBrowser,
    didNotStartBrowsingForPeers error: any Error
)
```

## Parameters 

`browser`  

The browser object that failed to start browsing.

`error`  

An error object indicating what went wrong.

