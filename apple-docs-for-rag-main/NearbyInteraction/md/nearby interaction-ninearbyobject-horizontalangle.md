

- Nearby Interaction
- NINearbyObject
-  horizontalAngle 

Instance Property

# horizontalAngle

An angle in radians that indicates the azimuthal direction to the nearby object.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+watchOS 9.0+

``` source
var horizontalAngle: Float? { get }
```

## Mentioned in 

Initiating and maintaining a session

## Discussion

The framework sets a value of this property when isCameraAssistanceEnabled is `true`.

This property is `nil` when direction is unavailable, such as when the app runs on Apple Watch.

## See Also

### Acquiring relative direction

var direction: simd_float3?

A vector that points from the user’s device in the direction of the peer device.

var verticalDirectionEstimate: NINearbyObject.VerticalDirectionEstimate

The estimation of a nearby object’s vertical position as it relates to the user’s device.

enum VerticalDirectionEstimate

Estimations of a nearby object’s vertical position in relation to the user’s device.

