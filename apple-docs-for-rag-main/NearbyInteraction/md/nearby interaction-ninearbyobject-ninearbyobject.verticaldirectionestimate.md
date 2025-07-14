

- Nearby Interaction
- NINearbyObject
-  NINearbyObject.VerticalDirectionEstimate 

Enumeration

# NINearbyObject.VerticalDirectionEstimate

Estimations of a nearby object’s vertical position in relation to the user’s device.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+watchOS 9.0+

``` source
enum VerticalDirectionEstimate
```

## Overview

The framework sets a nearby object’s verticalDirectionEstimate to an option of this enumeration when isCameraAssistanceEnabled is `true`.

## Topics

### Relative vertical location

case unknown

An indication that the nearby object resides at an unknown vertical location.

case same

An indication that the nearby object resides at an equivalent vertical location as the user’s device.

case above

An indication that the nearby object resides at a higher vertical location than the user’s device.

case below

An indication that the nearby object resides at a lower vertical location than the user’s device.

case aboveOrBelow

An indication that the nearby object doesn’t reside at the same vertical location as the user’s device.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Acquiring relative direction

var direction: simd_float3?

A vector that points from the user’s device in the direction of the peer device.

var horizontalAngle: Float?

An angle in radians that indicates the azimuthal direction to the nearby object.

var verticalDirectionEstimate: NINearbyObject.VerticalDirectionEstimate

The estimation of a nearby object’s vertical position as it relates to the user’s device.

