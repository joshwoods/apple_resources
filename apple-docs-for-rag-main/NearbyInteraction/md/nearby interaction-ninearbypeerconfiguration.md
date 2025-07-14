

- Nearby Interaction
-  NINearbyPeerConfiguration 

Class

# NINearbyPeerConfiguration

A configuration that enables interaction between iPhone or Apple Watch devices.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+watchOS 7.3+

``` source
class NINearbyPeerConfiguration
```

## Mentioned in 

Initiating and maintaining a session

## Overview

A peer interaction session enables two Apple devices to share their respective distance and direction through the device’s Ultra Wideband (UWB) chip. To start a peer interaction session, create a NINearbyPeerConfiguration instance and pass it to an NISession instance with the run(_:) function.

For an example app that demonstrates this configuration, see Implementing Interactions Between Users in Close Proximity.

### Enable Precision Finding for stationary objects

In iOS 16, you can combine the visual spatial power of ARKit with the radio sensitivity of the UWB chip to locate stationary nearby objects with considerable precision. To do that, set isCameraAssistanceEnabled to `true` and optionally provide the interaction session with an ARSession instance through setARSession(_:) before running the session. Together, the UWB chip and ARKit’s assistance enable Nearby Interaction to provide the same Precision Finding capabilities present in AirTag.

## Topics

### Creating a configuration

init(peerToken: NIDiscoveryToken)

Creates a configuration for interaction between devices, including iPhone and Apple Watch.

### Accessing the discovery token

var peerDiscoveryToken: NIDiscoveryToken

A value that uniquely identifies the other peer in the interaction session.

### Subclassing a configuration

class NIConfiguration

An abstract base class for interaction configurations.

### Enabling Camera Assistance

var isCameraAssistanceEnabled: Bool

A Boolean value that combines the spatial awareness of ARKit with Nearby Interaction to improve the accuracy of a nearby object’s position.

### Checking distance measurement capability

var isExtendedDistanceMeasurementEnabled: Bool

A Boolean value that indicates whether both peers can use extended distance measurement for this Nearby Interaction session instance.

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

### Phone interaction

Implementing Interactions Between Users in Close Proximity

Enable devices to access relative positioning information.

Discovering peers with Multipeer Connectivity

Exchange discovery tokens over the local network.

