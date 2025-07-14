

- ARKit
- ARGeoTrackingConfiguration
-  planeDetection 

Instance Property

# planeDetection

A value that specifies whether and how the session automatically attempts to detect flat surfaces in the camera-captured image.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var planeDetection: ARWorldTrackingConfiguration.PlaneDetection { get set }
```

## Discussion

By default, this configuration disables plane detection. If you enable horizontal or vertical plane detection, the session adds ARPlaneAnchor objects and notifies your ARSessionDelegate, ARSCNViewDelegate, or ARSKViewDelegate object when its analysis of captured video images detects an area that appears to be a flat surface.

## See Also

### Tracking Surfaces

struct PlaneDetection

Options for whether and how the framework detects flat surfaces in captured images.

