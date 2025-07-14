

- ARKit
- ARObjectScanningConfiguration
-  planeDetection 

Instance Property

# planeDetection

A value specifying whether and how the session attempts to automatically detect flat surfaces in the camera-captured image.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var planeDetection: ARWorldTrackingConfiguration.PlaneDetection { get set }
```

## Discussion

By default, plane detection is off. If you enable horizontal or vertical plane detection, the session adds ARPlaneAnchor objects and notifies your ARSessionDelegate, ARSCNViewDelegate, or ARSKViewDelegate object whenever its analysis of captured video images detects an area that appears to be a flat surface.

In an object-scanning session, you can use detected planes to help determine where the origin (anchor point) for a scanned object should be relative to its extent.

## See Also

### Enabling Plane Detection

struct PlaneDetection

Options for whether and how the framework detects flat surfaces in captured images.

