

- ARKit
- ARCamera
-  transform 

Instance Property

# transform

The position and orientation of the camera in world coordinate space.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
var transform: simd_float4x4 { get }
```

## Mentioned in 

Managing Session Life Cycle and Tracking Quality

## Discussion

World coordinate space in ARKit always follows a right-handed convention, but is oriented based on the session configuration. For details, see Understanding World Tracking.

This transform creates a local coordinate space for the camera that is constant with respect to device orientation. In camera space, the x-axis points to the right when the device is in UIDeviceOrientation.landscapeRight orientation—that is, the x-axis always points along the long axis of the device, from the front-facing camera toward the Home button. The y-axis points upward (with respect to UIDeviceOrientation.landscapeRight orientation), and the z-axis points away from the device on the screen side.

## See Also

### Examining Camera Geometry

var eulerAngles: simd_float3

The orientation of the camera, expressed as roll, pitch, and yaw values.

