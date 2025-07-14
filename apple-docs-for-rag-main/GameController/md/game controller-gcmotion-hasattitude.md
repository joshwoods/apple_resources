

- Game Controller
- GCMotion
-  hasAttitude 

Instance Property

# hasAttitude

A Boolean value that indicates whether the controller provides attitude data.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var hasAttitude: Bool { get }
```

## Discussion

true if the controller provides attitude data; otherwise, false.

## See Also

### Related Documentation

var attitude: GCQuaternion

The attitude of the controller.

### Verifying Capabilities

var hasRotationRate: Bool

A Boolean value that indicates whether the controller provides rotation data.

var hasGravityAndUserAcceleration: Bool

A Boolean value that indicates whether the controller provides gravity and user acceleration data.

var hasAttitudeAndRotationRate: Bool

A Boolean value that indicates whether the controller provides attitude and rotation data.

Deprecated

