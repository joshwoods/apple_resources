

- AVFoundation
- AVMetadataFaceObject
-  yawAngle 

Instance Property

# yawAngle

The yaw angle of the face specified in degrees.

iOS 6.0+iPadOS 6.0+Mac Catalyst 14.0+macOS 10.10+tvOS 9.0+

``` source
var yawAngle: CGFloat { get }
```

## Discussion

The yaw angle represents the rotation of the face around the vertical axis. A value of `0.0` yields a face that is looking directly at the camera, whereas a yaw angle of `90` degrees yields a face whose eye line is perpendicular to that of the camera.

You must check the value of the hasYawAngle property before accessing this property. If the value in the hasYawAngle property is false, reading the value in this property raises an exception.

## See Also

### Accessing the Face Detection Data

var hasRollAngle: Bool

A Boolean value indicating whether there is a valid roll angle associated with the face.

var rollAngle: CGFloat

The roll angle of the face specified in degrees.

var hasYawAngle: Bool

A Boolean value indicating whether there is a valid yaw angle associated with the face.

