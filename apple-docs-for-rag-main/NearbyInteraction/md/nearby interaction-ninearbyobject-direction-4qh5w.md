

- Nearby Interaction
- NINearbyObject
-  direction 

Instance Property

# direction

A vector that points from the user’s device in the direction of the peer device.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.4+watchOS 7.3+

``` source
var direction: simd_float3? { get }
```

## Mentioned in 

Initiating and maintaining a session

## Discussion

This property is `nil` when direction is unavailable, such as when the app runs on Apple Watch.

On iPhone, it’s possible to recieve direction for nearby third-party accessories in sessions that enable isCameraAssistanceEnabled.

### Interpret Direction

This property is a Cartesian triplet (x,y,z) in normalized units with a range of `[0..1]`. Nearby Interaction models direction as a coordinate on a sphere, such that a ray cast from the sphere’s center through the coordinate points toward the peer device. For each axis, the sphere center is at coordinate 0, and the surface is at coordinate 1. As the user looks at the device’s screen,

- The x-axis extends positively to the right.

- The y-axis extends positively upward.

- The z-axis extends negatively from the device’s center, away from the user.

The following figure illustrates the direction-vector coordinate space from two different angles.

For more information, see Initiating and maintaining a session.

## See Also

### Acquiring relative direction

var horizontalAngle: Float?

An angle in radians that indicates the azimuthal direction to the nearby object.

var verticalDirectionEstimate: NINearbyObject.VerticalDirectionEstimate

The estimation of a nearby object’s vertical position as it relates to the user’s device.

enum VerticalDirectionEstimate

Estimations of a nearby object’s vertical position in relation to the user’s device.

