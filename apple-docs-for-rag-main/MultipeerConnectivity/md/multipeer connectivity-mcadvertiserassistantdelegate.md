

- Multipeer Connectivity
-  MCAdvertiserAssistantDelegate 

Protocol

# MCAdvertiserAssistantDelegate

The `MCAdvertiserAssistantDelegate` protocol describes the methods that the delegate object for an `MCAdvertiserAssistant` instance can implement to handle advertising-related events.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.0+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
protocol MCAdvertiserAssistantDelegate : NSObjectProtocol
```

## Overview

No assumption should be made about which queue the delegate methods are called on. It is the delegate’s responsibility to ensure that any UIKit-related updates are called on the main thread.

## Topics

### Advertiser Assistant Delegate Methods

func advertiserAssistantWillPresentInvitation(MCAdvertiserAssistant)

Indicates that the advertiser assistant is about to present an invitation to the user.

func advertiserAssistantDidDismissInvitation(MCAdvertiserAssistant)

Indicates that the advertiser assistant finished showing the invitation to the user.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Protocols

protocol MCBrowserViewControllerDelegate

The `MCBrowserViewControllerDelegate` protocol defines the methods that your delegate object can implement to handle events related to the `MCBrowserViewController` class.

protocol MCNearbyServiceAdvertiserDelegate

The `MCNearbyServiceAdvertiserDelegate` protocol describes the methods that the delegate object for an `MCNearbyServiceAdvertiser` instance can implement for handling events from the `MCNearbyServiceAdvertiser` class.

protocol MCNearbyServiceBrowserDelegate

The `MCNearbyServiceBrowserDelegate` protocol defines methods that a `MCNearbyServiceBrowser` object’s delegate can implement to handle browser-related events.

protocol MCSessionDelegate

The `MCSessionDelegate` protocol defines methods that a delegate of the `MCSession` class can implement to handle session-related events. For more information, see MCSession.

