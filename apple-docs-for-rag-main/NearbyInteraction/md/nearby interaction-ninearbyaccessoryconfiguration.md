

- Nearby Interaction
-  NINearbyAccessoryConfiguration 

Class

# NINearbyAccessoryConfiguration

A configuration that enables interaction between iPhone and third-party accessories.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+watchOS 8.0+

``` source
class NINearbyAccessoryConfiguration
```

## Mentioned in 

Initiating and maintaining a session

## Overview

Use this class to interact with a third-party accessory that you partner with or develop.

For an example app that demonstrates this configuration, see Implementing spatial interactions with third-party accessories.

### Discover the accessory and create a configuration

To begin the interaction, your app discovers the nearby accessory using a technology you choose — like Core Bluetooth, the local network, or a secure internet connection — and establishes a two-way data link.

Over the data link, the accessory sends your app configuration data for this property’s init(data:) initializer. The accessory formats the data according to the Ultra Wideband (UWB) third-party device specification.

### Enable background interaction for Bluetooth accessories

In iOS 16, third-party UWB accessories paired to the device through Bluetooth can interact with your app while it’s in the background. This enables a new class of hands-free experiences. For example, the user’s phone can be in their pocket and prompt an eBike to power on when mounted, or prompt lights to turn on and music to play as the user enters a room.

To enable background interaction:

- The accessory implements the Bluetooth requirements described in the UWB third-party device specification.

- The app connects and pairs to the accessory using Core Bluetooth.

- The app calls the init(accessoryData:bluetoothPeerIdentifier:) initializer and passes in the accessory’s Bluetooth identifier.

### Start a session and share configuration data

To start a session, the app creates an NISession instance and passes an instance of this class into the session’s run(_:) function. After your app sets the session delegate, the system invokes the delegate’s session(_:didGenerateShareableConfigurationData:for:) callback and provides your device’s configuration data.

Over the data link, your app sends your device’s configuration data to the accessory, which enables the two devices to start receiving location updates. When the system gathers location updates for the accessory, Nearby Interaction calls your delegate’s session(_:didUpdate:) implementation. To match distance updates that your app receives through session(_:didUpdate:) with the accessory, compare the argument object’s discovery token with the value of this property’s accessoryDiscoveryToken.

### Enable Precision Finding for stationary objects

In iOS 16, you can combine the visual-spatial power of ARKit with the radio sensitivity of the Ultra Wideband (UWB) chip to locate stationary nearby objects with considerable precision. To do that, set isCameraAssistanceEnabled to `true` and optionally provide the interaction session with an ARSession instance through setARSession(_:) before running the session. Together, the UWB chip and ARKit’s assistance enable Nearby Interaction to provide the same Precision Finding capabilities present in AirTag.

## Topics

### Creating a configuration

init(data: Data) throws

Creates a configuration for interaction between iPhone and third-party accessories.

init(accessoryData: Data, bluetoothPeerIdentifier: UUID) throws

Creates a configuration for an accessory with the given Bluetooth peer identifier.

### Identifying the peer

var accessoryDiscoveryToken: NIDiscoveryToken

An identifier for the accessory in a session.

### Enabling Camera Assistance

var isCameraAssistanceEnabled: Bool

A Boolean value that combines the spatial awareness of ARKit with Nearby Interaction to improve the accuracy of a nearby object’s position.

## Relationships

### Inherits From

- NIConfiguration

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Third-party accessories

Extending advanced direction finding and ranging

Extend your app’s direction finding capabilities with data from Ultra Wideband devices.

Implementing spatial interactions with third-party accessories

Establish a connection with a nearby accessory to receive periodic measurements of its distance from the user.

