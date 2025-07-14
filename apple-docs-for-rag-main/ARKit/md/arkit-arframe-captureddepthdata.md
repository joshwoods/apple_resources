

- ARKit
- ARFrame
-  capturedDepthData 

Instance Property

# capturedDepthData

Depth data captured in front-camera experiences.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
var capturedDepthData: AVDepthData? { get }
```

## Discussion

Frames vended by the session contain a depth map captured by the depth sensor in addition to the color pixel buffer (see capturedImage) captured by the color camera. The depth-sensing camera provides data at a different frame rate than the color camera, so this property’s value can be `nil` if no depth data was captured at the same time as the current color image.

This depth data is available only in face-based experiences (see ARFaceTrackingConfiguration) using the device’s front TrueDepth camera. This property’s value is `nil` when running other AR configurations.

## See Also

### Accessing scene data

var lightEstimate: ARLightEstimate?

An estimate of lighting conditions based on the camera image.

func displayTransform(for: UIInterfaceOrientation, viewportSize: CGSize) -> CGAffineTransform

Returns an affine transform for converting between normalized image coordinates and a coordinate space appropriate for rendering the camera image onscreen.

var rawFeaturePoints: ARPointCloud?

The current intermediate results of the scene analysis ARKit uses to perform world tracking.

var capturedDepthDataTimestamp: TimeInterval

The time at which depth data for the frame (if any) was captured.

var sceneDepth: ARDepthData?

Data on the distance between a device’s rear camera and real-world objects in an AR experience.

var smoothedSceneDepth: ARDepthData?

An average of distance measurements between a device’s rear camera and real-world objects that creates smoother visuals in an AR experience.

