

- Game Controller
- GCMotion
-  attitude 

Instance Property

# attitude

The attitude of the controller.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var attitude: GCQuaternion { get }
```

## Discussion

The *attitude* is the orientation of a body relative to the controller’s reference frame.

## See Also

### Accessing Attitude and Rotation Data

struct GCQuaternion

A quaternion that represents a controller’s measurement of attitude.

var rotationRate: GCRotationRate

The rotation rate of the controller.

struct GCRotationRate

A structure that represents rotation rates around the x, y, and z axes.

struct GCEulerAngles

A structure that specifies the controller’s attitude as a series of rotations around the x, y, and z axes.

