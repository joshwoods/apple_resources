

- Game Controller
- GCMotion
-  hasGravityAndUserAcceleration 

Instance Property

# hasGravityAndUserAcceleration

A Boolean value that indicates whether the controller provides gravity and user acceleration data.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var hasGravityAndUserAcceleration: Bool { get }
```

## Discussion

true if the controller provides both gravity and user acceleration data; otherwise, false.

## See Also

### Related Documentation

var gravity: GCAcceleration

The gravity acceleration vector from the controller’s reference frame.

var userAcceleration: GCAcceleration

The acceleration that the user applies to the controller.

### Verifying Capabilities

var hasAttitude: Bool

A Boolean value that indicates whether the controller provides attitude data.

var hasRotationRate: Bool

A Boolean value that indicates whether the controller provides rotation data.

var hasAttitudeAndRotationRate: Bool

A Boolean value that indicates whether the controller provides attitude and rotation data.

Deprecated

