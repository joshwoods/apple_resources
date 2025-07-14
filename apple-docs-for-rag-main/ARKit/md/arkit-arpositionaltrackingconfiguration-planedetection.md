

- ARKit
- ARPositionalTrackingConfiguration
-  planeDetection 

Instance Property

# planeDetection

A value that specifies if and how the session automatically attempts to detect flat surfaces in the camera-captured image.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var planeDetection: ARWorldTrackingConfiguration.PlaneDetection { get set }
```

## Discussion

By default, this configuration disables plane detection. If you enable horizontal or vertical plane detection, the session adds ARPlaneAnchor objects and notifies your ARSessionDelegate, ARSCNViewDelegate, or ARSKViewDelegate object when its analysis of captured video images detects an area that appears to be a flat surface.

