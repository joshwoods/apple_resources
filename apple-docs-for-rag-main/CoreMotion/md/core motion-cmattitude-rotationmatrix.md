

- Core Motion
- CMAttitude
-  rotationMatrix 

Instance Property

# rotationMatrix

Returns a rotation matrix representing the device’s attitude.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+watchOS 2.0+

``` source
var rotationMatrix: CMRotationMatrix { get }
```

## Discussion

A rotation matrix in linear algebra describes the rotation of a body in three-dimensional Euclidean space.

## See Also

### Related Documentation

var quaternion: CMQuaternion

Returns a quaternion representing the device’s attitude.

### Getting a Mathematical Representation of Attitude as a Rotation Matrix

struct CMRotationMatrix

The type of a structure representing a rotation matrix.

