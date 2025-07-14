

- Game Controller
-  GCEulerAngles 

Structure

# GCEulerAngles

A structure that specifies the controller’s attitude as a series of rotations around the x, y, and z axes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
struct GCEulerAngles
```

## Topics

### Getting Euler Angle Values

var pitch: Double

The pitch of the controller in radians.

var yaw: Double

The yaw of the device in radians.

var roll: Double

The roll of the controller in radians.

### Initializers

init()

Creates the Euler angles structure.

init(pitch: Double, yaw: Double, roll: Double)

Creates the structure with the specified values.

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

struct GCRotationRate

A structure that represents rotation rates around the x, y, and z axes.

