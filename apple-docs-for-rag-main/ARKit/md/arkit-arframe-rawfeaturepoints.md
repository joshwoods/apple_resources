

- ARKit
- ARFrame
-  rawFeaturePoints 

Instance Property

# rawFeaturePoints

The current intermediate results of the scene analysis ARKit uses to perform world tracking.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
var rawFeaturePoints: ARPointCloud? { get }
```

## Discussion

These points represent notable features detected in the camera image. Their positions in 3D world coordinate space are extrapolated as part of the image analysis that ARKit performs in order to accurately track the device’s position, orientation, and movement. Taken together, these points loosely correlate to the contours of real-world objects in view of the camera.

ARKit does not guarantee that the number and arrangement of raw feature points will remain stable between software releases, or even between subsequent frames in the same session. Regardless, the point cloud can sometimes prove useful when debugging your app’s placement of virtual objects into the real-world scene.

If you display AR content with SceneKit using the ARSCNView class, you can display this point cloud with the ARSCNDebugOptionShowFeaturePoints debug option.

Feature point detection requires a ARWorldTrackingConfiguration session.

## See Also

### Accessing scene data

var lightEstimate: ARLightEstimate?

An estimate of lighting conditions based on the camera image.

func displayTransform(for: UIInterfaceOrientation, viewportSize: CGSize) -> CGAffineTransform

Returns an affine transform for converting between normalized image coordinates and a coordinate space appropriate for rendering the camera image onscreen.

var capturedDepthData: AVDepthData?

Depth data captured in front-camera experiences.

var capturedDepthDataTimestamp: TimeInterval

The time at which depth data for the frame (if any) was captured.

var sceneDepth: ARDepthData?

Data on the distance between a device’s rear camera and real-world objects in an AR experience.

var smoothedSceneDepth: ARDepthData?

An average of distance measurements between a device’s rear camera and real-world objects that creates smoother visuals in an AR experience.

