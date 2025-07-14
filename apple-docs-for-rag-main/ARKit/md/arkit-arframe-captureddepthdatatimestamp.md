

- ARKit
- ARFrame
-  capturedDepthDataTimestamp 

Instance Property

# capturedDepthDataTimestamp

The time at which depth data for the frame (if any) was captured.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
var capturedDepthDataTimestamp: TimeInterval { get }
```

## Discussion

Face-based AR (see ARFaceTrackingConfiguration) uses the front-facing, depth-sensing camera on compatible devices. When running such a configuration, frames vended by the session contain a depth map captured by the depth camera in addition to the color pixel buffer (see capturedImage) captured by the color camera. This property’s value is always zero when running other AR configurations.

The depth-sensing camera provides data at a different frame rate than the color camera, so this property’s value may not exactly match the timestamp property for the image captured by the color camera, and can also be zero if no depth data was captured at the same time as the current color image.

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

var sceneDepth: ARDepthData?

Data on the distance between a device’s rear camera and real-world objects in an AR experience.

var smoothedSceneDepth: ARDepthData?

An average of distance measurements between a device’s rear camera and real-world objects that creates smoother visuals in an AR experience.

