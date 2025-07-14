

- ARKit
- ARHitTestResult
- ARHitTestResult.ResultType
-  featurePoint Deprecated

Type Property

# featurePoint

A point on a surface detected by ARKit, but not part of any detected planes.

iOS 11.0–14.0DeprecatediPadOS 11.0–14.0DeprecatedMac Catalyst 13.1–14.0Deprecated

``` source
static var featurePoint: ARHitTestResult.ResultType { get }
```

Deprecated

Use raycasting

## Discussion

During a world-tracking AR session, ARKit builds a coarse point cloud representing its rough understanding of the 3D world around the user (see rawFeaturePoints). Individual feature points represent parts of the camera image likely to be part of a real-world surface, but not necessarily a planar surface.

When you search using this hit-test option, ARKit finds the feature point nearest to the hit-test ray (the extension of the 2D hit-test point into 3D world space), then returns the point on the ray nearest to that feature point.

## See Also

### Result Types

static var estimatedHorizontalPlane: ARHitTestResult.ResultType

A point on a real-world planar surface detected during the search, whose orientation is perpendicular to gravity.

Deprecated

static var estimatedVerticalPlane: ARHitTestResult.ResultType

A point on a real-world planar surface detected during the search, whose orientation is parallel to gravity.

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

