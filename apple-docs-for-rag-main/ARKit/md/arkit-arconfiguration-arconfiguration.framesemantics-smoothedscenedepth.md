

- ARKit
- ARConfiguration
- ARConfiguration.FrameSemantics
-  smoothedSceneDepth 

Type Property

# smoothedSceneDepth

An option that provides the distance from the device to real-world objects, averaged across several frames.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
static var smoothedSceneDepth: ARConfiguration.FrameSemantics { get }
```

## Discussion

Enable this option on a world-tracking configuration (ARWorldTrackingConfiguration) to instruct ARKit to provide your app with the distance between the user’s device and the real-world objects pictured in the frame’s capturedImage. ARKit samples this distance using the LiDAR scanner and provides the results through the smoothedSceneDepth property on the session’s currentFrame.

To minimize the difference in LiDAR readings across frames, ARKit processes the data as an average. The averaged readings reduce flickering to create a smoother motion effect when depicting objects with depth, as demonstrated in Creating a fog effect using scene depth. Alternatively, to access a discrete LiDAR reading at the instant the framework creates the current frame, use sceneDepth.

ARKit supports scene depth only on LiDAR-capable devices, so call supportsFrameSemantics(_:) to ensure device support before attempting to enable scene depth.

## See Also

### Accessing Depth

static var sceneDepth: ARConfiguration.FrameSemantics

An option that provides the distance from the device to real-world objects viewed through the camera.

