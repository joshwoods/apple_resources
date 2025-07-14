

- ARKit
- ARHitTestResult
- ARHitTestResult.ResultType
-  existingPlane Deprecated

Type Property

# existingPlane

A point on a real-world plane (already detected with the planeDetection option), without considering the plane’s size.

iOS 11.0–14.0DeprecatediPadOS 11.0–14.0DeprecatedMac Catalyst 13.1–14.0Deprecated

``` source
static var existingPlane: ARHitTestResult.ResultType { get }
```

Deprecated

Use raycasting

## Discussion

When searching for this result type, ARKit can return any point coplanar with an already detected plane, regardless of whether that plane’s already detected extent or geometry includes that point. (That is, this result type searches the infinite extensions of detected planes.)

An existing plane search can return any number of results, depending on how many already-detected planes the hit test ray intersects (if any).

## See Also

### Result Types

static var featurePoint: ARHitTestResult.ResultType

A point on a surface detected by ARKit, but not part of any detected planes.

Deprecated

static var estimatedHorizontalPlane: ARHitTestResult.ResultType

A point on a real-world planar surface detected during the search, whose orientation is perpendicular to gravity.

Deprecated

static var estimatedVerticalPlane: ARHitTestResult.ResultType

A point on a real-world planar surface detected during the search, whose orientation is parallel to gravity.

Deprecated

static var existingPlaneUsingExtent: ARHitTestResult.ResultType

A point on a real-world plane (already detected with the planeDetection option), respecting the plane’s estimated size.

Deprecated

static var existingPlaneUsingGeometry: ARHitTestResult.ResultType

A point on a real-world plane (already detected with the planeDetection option), respecting the plane’s estimated size and shape.

Deprecated

