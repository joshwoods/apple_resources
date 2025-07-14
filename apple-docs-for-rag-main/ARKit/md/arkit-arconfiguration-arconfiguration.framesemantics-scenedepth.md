

- ARKit
- ARConfiguration
- ARConfiguration.FrameSemantics
-  sceneDepth 

Type Property

# sceneDepth

An option that provides the distance from the device to real-world objects viewed through the camera.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
static var sceneDepth: ARConfiguration.FrameSemantics { get }
```

## Discussion

Enable this option on a world-tracking configuration (ARWorldTrackingConfiguration) to instruct ARKit to provide your app with the distance between the user’s device and the real-world objects in the camera feed. ARKit samples this distance using the LiDAR scanner and provides the results through the sceneDepth property on the session’s currentFrame.

ARKit creates this object from LiDAR readings at same time as the current frame. The data in sceneDepth reflects the distance from the device to real-world objects pictured in the frame’s capturedImage. Alternatively, ARKit provides a smoothedSceneDepth property that minimizes the difference in LiDAR readings across frames.

ARKit supports scene depth only on LiDAR-capable devices, so call supportsFrameSemantics(_:) to ensure device support before attempting to enable scene depth.

## See Also

### Accessing Depth

static var smoothedSceneDepth: ARConfiguration.FrameSemantics

An option that provides the distance from the device to real-world objects, averaged across several frames.

