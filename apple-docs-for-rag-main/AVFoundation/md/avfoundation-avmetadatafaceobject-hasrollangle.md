

- AVFoundation
- AVMetadataFaceObject
-  hasRollAngle 

Instance Property

# hasRollAngle

A Boolean value indicating whether there is a valid roll angle associated with the face.

iOS 6.0+iPadOS 6.0+Mac Catalyst 14.0+macOS 10.10+tvOS 9.0+

``` source
var hasRollAngle: Bool { get }
```

## Discussion

If the value of this property is false, the value in the rollAngle property is invalid and must not be accessed.

## See Also

### Accessing the Face Detection Data

var rollAngle: CGFloat

The roll angle of the face specified in degrees.

var hasYawAngle: Bool

A Boolean value indicating whether there is a valid yaw angle associated with the face.

var yawAngle: CGFloat

The yaw angle of the face specified in degrees.

