

- Game Controller
- GCMotion
-  rotationRate 

Instance Property

# rotationRate

The rotation rate of the controller.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var rotationRate: GCRotationRate { get }
```

## Discussion

The *rotation rate* is a gyroscopic measurement of the controller’s rotation around the x, y, and z axes.

## See Also

### Accessing Attitude and Rotation Data

var attitude: GCQuaternion

The attitude of the controller.

struct GCQuaternion

A quaternion that represents a controller’s measurement of attitude.

struct GCRotationRate

A structure that represents rotation rates around the x, y, and z axes.

struct GCEulerAngles

A structure that specifies the controller’s attitude as a series of rotations around the x, y, and z axes.

