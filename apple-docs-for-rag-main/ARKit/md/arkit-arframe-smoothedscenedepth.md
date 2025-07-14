

- ARKit
- ARFrame
-  smoothedSceneDepth 

Instance Property

# smoothedSceneDepth

An average of distance measurements between a device’s rear camera and real-world objects that creates smoother visuals in an AR experience.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var smoothedSceneDepth: ARDepthData? { get }
```

## Discussion

This property describes the distance between a device’s camera and objects or areas in the real world, including ARKit’s confidence in the estimated distance. This is similar to sceneDepth except that the framework smoothes the depth data over time to lessen its frame-to-frame delta.

This property is `nil` by default. Add the smoothedSceneDepth frame semantic to your configuration’s frameSemantics to instruct the framework to populate this value with ARDepthData captured by the LiDAR scanner.

Call supportsFrameSemantics(_:) on your app’s configuration to support smoothed scene depth on select devices and configurations.

## See Also

### Accessing scene data

var lightEstimate: ARLightEstimate?

An estimate of lighting conditions based on the camera image.

func displayTransform(for: UIInterfaceOrientation, viewportSize: CGSize) -> CGAffineTransform

Returns an affine transform for converting between normalized image coordinates and a coordinate space appropriate for rendering the camera image onscreen.

var rawFeaturePoints: ARPointCloud?

The current intermediate results of the scene analysis ARKit uses to perform world tracking.

var capturedDepthData: AVDepthData?

Depth data captured in front-camera experiences.

var capturedDepthDataTimestamp: TimeInterval

The time at which depth data for the frame (if any) was captured.

var sceneDepth: ARDepthData?

Data on the distance between a device’s rear camera and real-world objects in an AR experience.

