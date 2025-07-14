

- ARKit
- ARConfiguration
- ARConfiguration.WorldAlignment
-  ARConfiguration.WorldAlignment.camera 

Case

# ARConfiguration.WorldAlignment.camera

The scene coordinate system is locked to match the orientation of the camera.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
case camera
```

## Discussion

Camera alignment defines a coordinate system based on the native sensor orientation of the device camera. Relative to a AVCaptureVideoOrientation.landscapeRight-oriented camera image, the x-axis points to the right, the y-axis points up, and the z-axis points out the front of the device (toward the user).

Note

This coordinate system is always the same regardless of device or user interface orientation. That is, the x-axis always points along the long axis of the device, even if that direction is “down” relative to the user.

When this alignment is active, ARKit performs no device motion tracking. That is, world-space positions are effectively always relative to the current position and orientation of the device. (For example, a SceneKit object placed in an ARSCNView will thus maintain the same position on screen, even as the camera image changes while the device moves.)

## See Also

### Alignments

case gravity

The coordinate system’s y-axis is parallel to gravity, and its origin is the initial position of the device.

case gravityAndHeading

The coordinate system’s y-axis is parallel to gravity, its x- and z-axes are oriented to compass heading, and its origin is the initial position of the device.

