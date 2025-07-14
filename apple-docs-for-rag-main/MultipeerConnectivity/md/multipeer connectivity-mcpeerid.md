

- Multipeer Connectivity
-  MCPeerID 

Class

# MCPeerID

An `MCPeerID` object represents a peer in a multipeer session.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
class MCPeerID
```

## Overview

You create a single peer ID object that represents the instance of your app running on the local device. The Multipeer Connectivity framework is responsible for creating peer ID objects that represent other devices.

To create a new peer ID for the local app and associate a display name with that ID, call init(displayName:). The peer’s name must be no longer than 63 bytes in UTF-8 encoding.

Each peer ID your app creates with init(displayName:) is unique, even when supplying the same display name. If you want a device’s peer ID to be stable over time, don’t create a new peer ID every time your app begins advertising or browsing. Instead, archive the ID when you create it, and then unarchive it the next time you need it. If you need the peer ID to be tied to the display name, you can archive the name as well, and only create a new peer ID when the name changes, as illustrated in the following code fragment:

```
```

## Topics

### Peer Methods

init(displayName: String)

Initializes a peer.

var displayName: String

The display name for this peer.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- SynchronizationPeerID

## See Also

### Classes

class MCAdvertiserAssistant

The `MCAdvertiserAssistant` is a convenience class that handles advertising, presents incoming invitations to the user, and handles users’ responses. Use this class to provide a user interface for handling invitations when your app does not require programmatic control over the invitation process.

class MCBrowserViewController

The `MCBrowserViewController` class presents nearby devices to the user and enables the user to invite nearby devices to a session. To use this class in iOS or tvOS, call methods from the underlying `UIViewController` class (prepare(for:sender:) and performSegue(withIdentifier:sender:) for storyboards or present(_:animated:completion:) and dismiss(animated:completion:) for nib-based views) to present and dismiss the view controller. In macOS, use the comparable `NSViewController` methods presentAsSheet(_:) and dismiss(_:) instead.

class MCNearbyServiceAdvertiser

The `MCNearbyServiceAdvertiser` class publishes an advertisement for a specific service that your app provides through the Multipeer Connectivity framework and notifies its delegate about invitations from nearby peers.

class MCNearbyServiceBrowser

Searches (by service type) for services offered by nearby devices using infrastructure Wi-Fi, peer-to-peer Wi-Fi, and Bluetooth (in iOS) or Ethernet (in macOS and tvOS), and provides the ability to easily invite those devices to a Multipeer Connectivity session (`MCSession`).

class MCSession

An `MCSession` object enables and manages communication among all peers in a Multipeer Connectivity session.

