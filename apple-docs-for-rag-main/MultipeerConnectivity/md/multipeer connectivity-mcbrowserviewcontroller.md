

- Multipeer Connectivity
-  MCBrowserViewController 

Class

# MCBrowserViewController

The `MCBrowserViewController` class presents nearby devices to the user and enables the user to invite nearby devices to a session. To use this class in iOS or tvOS, call methods from the underlying `UIViewController` class (prepare(for:sender:) and performSegue(withIdentifier:sender:) for storyboards or present(_:animated:completion:) and dismiss(animated:completion:) for nib-based views) to present and dismiss the view controller. In macOS, use the comparable `NSViewController` methods presentAsSheet(_:) and dismiss(_:) instead.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
class MCBrowserViewController
```

## Topics

### Initializing a Browser View Controller

convenience init(serviceType: String, session: MCSession)

Initializes a browser view controller using the provided service type and session.

init(browser: MCNearbyServiceBrowser, session: MCSession)

Initializes a browser view controller with the provided browser and session.

var delegate: (any MCBrowserViewControllerDelegate)?

The delegate object that handles browser-view-controller-related events.

var browser: MCNearbyServiceBrowser?

The browser object that is used for discovering peers.

var session: MCSession

The multipeer session to which the invited peers are connected.

### Getting and Setting the Maximum and Minimum Number of Peers

var maximumNumberOfPeers: Int

The maximum number of peers allowed in a session, including the local peer.

var minimumNumberOfPeers: Int

The minimum number of peers that need to be in a session, including the local peer.

## Relationships

### Inherits From

- NSViewController
- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MCNearbyServiceBrowserDelegate
- NSCoding
- NSEditor
- NSExtensionRequestHandling
- NSObjectProtocol
- NSSeguePerforming
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Classes

class MCAdvertiserAssistant

The `MCAdvertiserAssistant` is a convenience class that handles advertising, presents incoming invitations to the user, and handles users’ responses. Use this class to provide a user interface for handling invitations when your app does not require programmatic control over the invitation process.

class MCNearbyServiceAdvertiser

The `MCNearbyServiceAdvertiser` class publishes an advertisement for a specific service that your app provides through the Multipeer Connectivity framework and notifies its delegate about invitations from nearby peers.

class MCNearbyServiceBrowser

Searches (by service type) for services offered by nearby devices using infrastructure Wi-Fi, peer-to-peer Wi-Fi, and Bluetooth (in iOS) or Ethernet (in macOS and tvOS), and provides the ability to easily invite those devices to a Multipeer Connectivity session (`MCSession`).

class MCPeerID

An `MCPeerID` object represents a peer in a multipeer session.

class MCSession

An `MCSession` object enables and manages communication among all peers in a Multipeer Connectivity session.

