

- Game Controller
-  GCRotationRate 

Structure

# GCRotationRate

A structure that represents rotation rates around the x, y, and z axes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
struct GCRotationRate
```

## Topics

### Getting Rotation Rate Values

var x: Double

The rotation rate around the x-axis in radians per second.

var y: Double

The rotation rate around the y-axis in radians per second.

var z: Double

The rotation rate around the z-axis in radians per second.

### Initializers

init()

Creates a rotation rate structure.

init(x: Double, y: Double, z: Double)

Creates a rotation rate structure with the specified values.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Accessing Attitude and Rotation Data

var attitude: GCQuaternion

The attitude of the controller.

struct GCQuaternion

A quaternion that represents a controller’s measurement of attitude.

var rotationRate: GCRotationRate

The rotation rate of the controller.

struct GCEulerAngles

A structure that specifies the controller’s attitude as a series of rotations around the x, y, and z axes.

