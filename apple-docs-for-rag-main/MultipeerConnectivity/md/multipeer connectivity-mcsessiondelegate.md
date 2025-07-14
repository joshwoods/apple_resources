

- Multipeer Connectivity
-  MCSessionDelegate 

Protocol

# MCSessionDelegate

The `MCSessionDelegate` protocol defines methods that a delegate of the `MCSession` class can implement to handle session-related events. For more information, see MCSession.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.0+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
protocol MCSessionDelegate : NSObjectProtocol
```

## Overview

Delegate calls occur on a private serial queue. If your app needs to perform an action on a particular run loop or operation queue, its delegate method should explicitly dispatch or schedule that work.

## Topics

### MCSession Delegate Methods

func session(MCSession, didReceive: Data, fromPeer: MCPeerID)

Indicates that an `NSData` object has been received from a nearby peer.

**Required**

func session(MCSession, didStartReceivingResourceWithName: String, fromPeer: MCPeerID, with: Progress)

Indicates that the local peer began receiving a resource from a nearby peer.

**Required**

func session(MCSession, didFinishReceivingResourceWithName: String, fromPeer: MCPeerID, at: URL?, withError: (any Error)?)

Indicates that the local peer finished receiving a resource from a nearby peer.

**Required**

func session(MCSession, didReceive: InputStream, withName: String, fromPeer: MCPeerID)

Called when a nearby peer opens a byte stream connection to the local peer.

**Required**

func session(MCSession, peer: MCPeerID, didChange: MCSessionState)

Called when the state of a nearby peer changes.

**Required**

func session(MCSession, didReceiveCertificate: [Any]?, fromPeer: MCPeerID, certificateHandler: (Bool) -> Void)

Called to validate the client certificate provided by a peer when the connection is first established.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Protocols

protocol MCAdvertiserAssistantDelegate

The `MCAdvertiserAssistantDelegate` protocol describes the methods that the delegate object for an `MCAdvertiserAssistant` instance can implement to handle advertising-related events.

protocol MCBrowserViewControllerDelegate

The `MCBrowserViewControllerDelegate` protocol defines the methods that your delegate object can implement to handle events related to the `MCBrowserViewController` class.

protocol MCNearbyServiceAdvertiserDelegate

The `MCNearbyServiceAdvertiserDelegate` protocol describes the methods that the delegate object for an `MCNearbyServiceAdvertiser` instance can implement for handling events from the `MCNearbyServiceAdvertiser` class.

protocol MCNearbyServiceBrowserDelegate

The `MCNearbyServiceBrowserDelegate` protocol defines methods that a `MCNearbyServiceBrowser` object’s delegate can implement to handle browser-related events.

