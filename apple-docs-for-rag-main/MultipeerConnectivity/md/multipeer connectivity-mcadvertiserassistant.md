

- Multipeer Connectivity
-  MCAdvertiserAssistant 

Class

# MCAdvertiserAssistant

The `MCAdvertiserAssistant` is a convenience class that handles advertising, presents incoming invitations to the user, and handles users’ responses. Use this class to provide a user interface for handling invitations when your app does not require programmatic control over the invitation process.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
class MCAdvertiserAssistant
```

## Overview

Before you can advertise a service, you must create an `MCPeerID` object that identifies your app and the user to nearby devices.

## Topics

### Initializing and Configuring

init(serviceType: String, discoveryInfo: [String : String]?, session: MCSession)

Initializes an advertiser assistant object.

var session: MCSession

The session into which new peers are added after accepting an invitation.

var delegate: (any MCAdvertiserAssistantDelegate)?

The delegate object that handles advertising-assistant-related events.

var discoveryInfo: [String : String]?

The `info` dictionary that was passed when this object was initialized.

var serviceType: String

The service type that your app is advertising.

### Starting and Stopping the Assistant

func start()

Begins advertising the service provided by a local peer and starts the assistant.

func stop()

Stops advertising the service provided by a local peer and stops the assistant.

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

class MCBrowserViewController

The `MCBrowserViewController` class presents nearby devices to the user and enables the user to invite nearby devices to a session. To use this class in iOS or tvOS, call methods from the underlying `UIViewController` class (prepare(for:sender:) and performSegue(withIdentifier:sender:) for storyboards or present(_:animated:completion:) and dismiss(animated:completion:) for nib-based views) to present and dismiss the view controller. In macOS, use the comparable `NSViewController` methods presentAsSheet(_:) and dismiss(_:) instead.

class MCNearbyServiceAdvertiser

The `MCNearbyServiceAdvertiser` class publishes an advertisement for a specific service that your app provides through the Multipeer Connectivity framework and notifies its delegate about invitations from nearby peers.

class MCNearbyServiceBrowser

Searches (by service type) for services offered by nearby devices using infrastructure Wi-Fi, peer-to-peer Wi-Fi, and Bluetooth (in iOS) or Ethernet (in macOS and tvOS), and provides the ability to easily invite those devices to a Multipeer Connectivity session (`MCSession`).

class MCPeerID

An `MCPeerID` object represents a peer in a multipeer session.

class MCSession

An `MCSession` object enables and manages communication among all peers in a Multipeer Connectivity session.

