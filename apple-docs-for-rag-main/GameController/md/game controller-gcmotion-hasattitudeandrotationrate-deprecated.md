

- Game Controller
- GCMotion
-  hasAttitudeAndRotationRate Deprecated

Instance Property

# hasAttitudeAndRotationRate

A Boolean value that indicates whether the controller provides attitude and rotation data.

iOS 11.0–14.0DeprecatediPadOS 11.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.13–11.0DeprecatedtvOS 11.0–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var hasAttitudeAndRotationRate: Bool { get }
```

Deprecated

Use the hasAttitude and hasRotationRate methods instead.

## Discussion

true if the controller provides attitude and rotation rate data; otherwise, false.

## See Also

### Related Documentation

var attitude: GCQuaternion

The attitude of the controller.

var rotationRate: GCRotationRate

The rotation rate of the controller.

### Verifying Capabilities

var hasAttitude: Bool

A Boolean value that indicates whether the controller provides attitude data.

var hasRotationRate: Bool

A Boolean value that indicates whether the controller provides rotation data.

var hasGravityAndUserAcceleration: Bool

A Boolean value that indicates whether the controller provides gravity and user acceleration data.

