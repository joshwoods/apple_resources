

- Multipeer Connectivity
-  MCNearbyServiceBrowser 

Class

# MCNearbyServiceBrowser

Searches (by service type) for services offered by nearby devices using infrastructure Wi-Fi, peer-to-peer Wi-Fi, and Bluetooth (in iOS) or Ethernet (in macOS and tvOS), and provides the ability to easily invite those devices to a Multipeer Connectivity session (`MCSession`).

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
class MCNearbyServiceBrowser
```

## Topics

### Initializing the Browser

init(peer: MCPeerID, serviceType: String)

Initializes the nearby service browser object.

var delegate: (any MCNearbyServiceBrowserDelegate)?

The delegate object that handles browser-related events.

var myPeerID: MCPeerID

The local peer ID for this instance.

var serviceType: String

The service type to browse for.

### Browsing for Peers

func startBrowsingForPeers()

Starts browsing for peers.

func stopBrowsingForPeers()

Stops browsing for peers.

### Inviting Peers

func invitePeer(MCPeerID, to: MCSession, withContext: Data?, timeout: TimeInterval)

Invites a discovered peer to join a Multipeer Connectivity session.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Classes

class MCAdvertiserAssistant

The `MCAdvertiserAssistant` is a convenience class that handles advertising, presents incoming invitations to the user, and handles users’ responses. Use this class to provide a user interface for handling invitations when your app does not require programmatic control over the invitation process.

class MCBrowserViewController

The `MCBrowserViewController` class presents nearby devices to the user and enables the user to invite nearby devices to a session. To use this class in iOS or tvOS, call methods from the underlying `UIViewController` class (prepare(for:sender:) and performSegue(withIdentifier:sender:) for storyboards or present(_:animated:completion:) and dismiss(animated:completion:) for nib-based views) to present and dismiss the view controller. In macOS, use the comparable `NSViewController` methods presentAsSheet(_:) and dismiss(_:) instead.

class MCNearbyServiceAdvertiser

The `MCNearbyServiceAdvertiser` class publishes an advertisement for a specific service that your app provides through the Multipeer Connectivity framework and notifies its delegate about invitations from nearby peers.

class MCPeerID

An `MCPeerID` object represents a peer in a multipeer session.

class MCSession

An `MCSession` object enables and manages communication among all peers in a Multipeer Connectivity session.

