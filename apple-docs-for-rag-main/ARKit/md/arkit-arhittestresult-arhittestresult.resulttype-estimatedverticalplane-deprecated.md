

- ARKit
- ARHitTestResult
- ARHitTestResult.ResultType
-  estimatedVerticalPlane Deprecated

Type Property

# estimatedVerticalPlane

A point on a real-world planar surface detected during the search, whose orientation is parallel to gravity.

iOS 11.3–14.0DeprecatediPadOS 11.3–14.0DeprecatedMac Catalyst 13.1–14.0Deprecated

``` source
static var estimatedVerticalPlane: ARHitTestResult.ResultType { get }
```

## Discussion

ARKit provides two ways to locate real-world flat surfaces in a scene. *Plane detection* (enabled with planeDetection on your session configuration) is an ongoing process, continuously analyzing the scene to accurately map the position and extent of any planes in view. Because plane detection takes time, you can fall back to *plane estimation* to get an instant, but less accurate, indication of whether a 2D point in the camera image corresponds to a real-world flat surface.

Because plane detection results are more accurate than plane estimation results, ARKit prefers the former when searching for both. If your hit-test search includes both estimatedVerticalPlane and one or more existingPlane types, and the search finds any already detected plane anchors, the search returns only the existing plane(s) and no estimated plane.

An estimated plane search returns at most one result—the best estimate for a vertical plane intersecting the hit-test ray.

## See Also

### Result Types

static var featurePoint: ARHitTestResult.ResultType

A point on a surface detected by ARKit, but not part of any detected planes.

Deprecated

static var estimatedHorizontalPlane: ARHitTestResult.ResultType

A point on a real-world planar surface detected during the search, whose orientation is perpendicular to gravity.

Deprecated

static var existingPlane: ARHitTestResult.ResultType

A point on a real-world plane (already detected with the planeDetection option), without considering the plane’s size.

Deprecated

static var existingPlaneUsingExtent: ARHitTestResult.ResultType

A point on a real-world plane (already detected with the planeDetection option), respecting the plane’s estimated size.

Deprecated

static var existingPlaneUsingGeometry: ARHitTestResult.ResultType

A point on a real-world plane (already detected with the planeDetection option), respecting the plane’s estimated size and shape.

Deprecated

