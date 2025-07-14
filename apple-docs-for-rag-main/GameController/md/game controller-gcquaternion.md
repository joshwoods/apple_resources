

- Game Controller
-  GCQuaternion 

Structure

# GCQuaternion

A quaternion that represents a controller’s measurement of attitude.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
struct GCQuaternion
```

## Topics

### Getting Quaternion Values

var x: Double

The value for the x-axis of the quaternion.

var y: Double

The value for the y-axis of the quaternion.

var z: Double

The value for the z-axis of the quaternion.

var w: Double

The value for the w-axis of the quaternion.

### Initializers

init()

Creates a quaternion structure.

init(x: Double, y: Double, z: Double, w: Double)

Creates a quaternion structure with the specified values.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Accessing Attitude and Rotation Data

var attitude: GCQuaternion

The attitude of the controller.

var rotationRate: GCRotationRate

The rotation rate of the controller.

struct GCRotationRate

A structure that represents rotation rates around the x, y, and z axes.

struct GCEulerAngles

A structure that specifies the controller’s attitude as a series of rotations around the x, y, and z axes.

