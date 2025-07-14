

- Multipeer Connectivity
-  MCBrowserViewControllerDelegate 

Protocol

# MCBrowserViewControllerDelegate

The `MCBrowserViewControllerDelegate` protocol defines the methods that your delegate object can implement to handle events related to the `MCBrowserViewController` class.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.0+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
protocol MCBrowserViewControllerDelegate : NSObjectProtocol
```

## Overview

No assumption should be made about which queue the delegate methods are called on. It is the receiver’s responsibility to ensure that any UIKit-related updates are called on the main thread.

## Topics

### Peer Notifications

func browserViewController(MCBrowserViewController, shouldPresentNearbyPeer: MCPeerID, withDiscoveryInfo: [String : String]?) -> Bool

Called when a new peer is discovered to decide whether to show it in the user interface.

### User Action Notifications

func browserViewControllerDidFinish(MCBrowserViewController)

Called when the browser view controller is dismissed with peers connected in a session.

**Required**

func browserViewControllerWasCancelled(MCBrowserViewController)

Called when the user cancels the browser view controller.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Protocols

protocol MCAdvertiserAssistantDelegate

The `MCAdvertiserAssistantDelegate` protocol describes the methods that the delegate object for an `MCAdvertiserAssistant` instance can implement to handle advertising-related events.

protocol MCNearbyServiceAdvertiserDelegate

The `MCNearbyServiceAdvertiserDelegate` protocol describes the methods that the delegate object for an `MCNearbyServiceAdvertiser` instance can implement for handling events from the `MCNearbyServiceAdvertiser` class.

protocol MCNearbyServiceBrowserDelegate

The `MCNearbyServiceBrowserDelegate` protocol defines methods that a `MCNearbyServiceBrowser` object’s delegate can implement to handle browser-related events.

protocol MCSessionDelegate

The `MCSessionDelegate` protocol defines methods that a delegate of the `MCSession` class can implement to handle session-related events. For more information, see MCSession.

