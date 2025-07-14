

- Multipeer Connectivity
-  MCNearbyServiceBrowserDelegate 

Protocol

# MCNearbyServiceBrowserDelegate

The `MCNearbyServiceBrowserDelegate` protocol defines methods that a `MCNearbyServiceBrowser` object’s delegate can implement to handle browser-related events.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.0+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
protocol MCNearbyServiceBrowserDelegate : NSObjectProtocol
```

## Overview

No assumption should be made about which queue the delegate methods are called on. It is the receiver’s responsibility to ensure that any `UIKit` updates are called on the main thread.

## Topics

### Error Handling Delegate Methods

func browser(MCNearbyServiceBrowser, didNotStartBrowsingForPeers: any Error)

Called when a browser failed to start browsing for peers.

### Peer Discovery Delegate Methods

func browser(MCNearbyServiceBrowser, foundPeer: MCPeerID, withDiscoveryInfo: [String : String]?)

Called when a nearby peer is found.

**Required**

func browser(MCNearbyServiceBrowser, lostPeer: MCPeerID)

Called when a nearby peer is lost.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- MCBrowserViewController

## See Also

### Protocols

protocol MCAdvertiserAssistantDelegate

The `MCAdvertiserAssistantDelegate` protocol describes the methods that the delegate object for an `MCAdvertiserAssistant` instance can implement to handle advertising-related events.

protocol MCBrowserViewControllerDelegate

The `MCBrowserViewControllerDelegate` protocol defines the methods that your delegate object can implement to handle events related to the `MCBrowserViewController` class.

protocol MCNearbyServiceAdvertiserDelegate

The `MCNearbyServiceAdvertiserDelegate` protocol describes the methods that the delegate object for an `MCNearbyServiceAdvertiser` instance can implement for handling events from the `MCNearbyServiceAdvertiser` class.

protocol MCSessionDelegate

The `MCSessionDelegate` protocol defines methods that a delegate of the `MCSession` class can implement to handle session-related events. For more information, see MCSession.

