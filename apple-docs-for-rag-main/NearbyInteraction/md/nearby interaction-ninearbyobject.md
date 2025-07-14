

- Nearby Interaction
-  NINearbyObject 

Class

# NINearbyObject

Location information for a peer device in an interaction session.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+watchOS 7.3+

``` source
class NINearbyObject
```

## Overview

A nearby object refers to a peer Apple device or third-party accessory.

When the framework is ready to provide your app with information about a nearby object’s relative position, it calls your delegate’s session(_:didUpdate:) implementation.

If a session can’t provide peer direction or distance, it sets the values to `nil`. In Objective-C, the session uses the NINearbyObjectDirectionNotAvailable and NINearbyObjectDistanceNotAvailable values to indicate missing direction or distance.

For more information, see Initiating and maintaining a session.

## Topics

### Identifying a nearby device

var discoveryToken: NIDiscoveryToken

A unique identifier for a peer device in the session.

### Acquring relative distance

var distance: Float?

The distance from the user’s device to the peer device in meters.

### Acquiring relative direction

var direction: simd_float3?

A vector that points from the user’s device in the direction of the peer device.

var horizontalAngle: Float?

An angle in radians that indicates the azimuthal direction to the nearby object.

var verticalDirectionEstimate: NINearbyObject.VerticalDirectionEstimate

The estimation of a nearby object’s vertical position as it relates to the user’s device.

enum VerticalDirectionEstimate

Estimations of a nearby object’s vertical position in relation to the user’s device.

### Explaining participation

enum RemovalReason

The reason a session removed a nearby object.

## Relationships

### Inherits From

- NSObject

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

### Periodic updates

protocol NISessionDelegate

An object that monitors and reacts to session updates.

