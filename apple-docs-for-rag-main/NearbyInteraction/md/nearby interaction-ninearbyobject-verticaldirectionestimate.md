

- Nearby Interaction
- NINearbyObject
-  verticalDirectionEstimate 

Instance Property

# verticalDirectionEstimate

The estimation of a nearby object’s vertical position as it relates to the user’s device.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+watchOS 9.0+

``` source
var verticalDirectionEstimate: NINearbyObject.VerticalDirectionEstimate { get }
```

## Mentioned in 

Initiating and maintaining a session

## Discussion

The framework sets a value of this property when isCameraAssistanceEnabled is `true`.

The framework periodically sets the value of this property when vertical positioning is available. Otherwise, the framework sets the value to NINearbyObject.VerticalDirectionEstimate.unknown.

## See Also

### Acquiring relative direction

var direction: simd_float3?

A vector that points from the user’s device in the direction of the peer device.

var horizontalAngle: Float?

An angle in radians that indicates the azimuthal direction to the nearby object.

enum VerticalDirectionEstimate

Estimations of a nearby object’s vertical position in relation to the user’s device.

