

- ARKit
- ARFrame
-  lightEstimate 

Instance Property

# lightEstimate

An estimate of lighting conditions based on the camera image.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
var lightEstimate: ARLightEstimate? { get }
```

## Discussion

If you render your own overlay graphics for the AR scene, you can use this information in shading algorithms to help make those graphics match the real-world lighting conditions of the scene captured by the camera. (The ARSCNView class automatically uses this information to configure SceneKit lighting.)

This property’s value is `nil` if the isLightEstimationEnabled property of the session configuration that captured this frame is false.

## See Also

### Accessing scene data

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

var smoothedSceneDepth: ARDepthData?

An average of distance measurements between a device’s rear camera and real-world objects that creates smoother visuals in an AR experience.

