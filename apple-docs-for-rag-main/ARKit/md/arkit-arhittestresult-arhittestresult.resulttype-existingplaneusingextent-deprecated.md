

- ARKit
- ARHitTestResult
- ARHitTestResult.ResultType
-  existingPlaneUsingExtent Deprecated

Type Property

# existingPlaneUsingExtent

A point on a real-world plane (already detected with the planeDetection option), respecting the plane’s estimated size.

iOS 11.0–14.0DeprecatediPadOS 11.0–14.0DeprecatedMac Catalyst 13.1–14.0Deprecated

``` source
static var existingPlaneUsingExtent: ARHitTestResult.ResultType { get }
```

Deprecated

Use raycasting

## Discussion

When searching for this result type, ARKit returns a point coplanar with an already detected plane only if that point lies within the area defined by the plane’s center and extent properties. Those properties (together with the anchor’s transform) define the smallest rectangular area that includes all regions ARKit estimates to be a part of the plane.

However, that rectangular area may contain regions that are not part of the same real-world surface. There may also be parts of the same real-world surface that lie outside the rectangle because ARKit has not yet recognized them as part of the same plane. You can get a more precise estimate of the plane area ARKit has recognized by testing with the existingPlaneUsingGeometry type, or extend your hit test to an infinite plane with the existingPlane type.

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

static var existingPlane: ARHitTestResult.ResultType

A point on a real-world plane (already detected with the planeDetection option), without considering the plane’s size.

Deprecated

static var existingPlaneUsingGeometry: ARHitTestResult.ResultType

A point on a real-world plane (already detected with the planeDetection option), respecting the plane’s estimated size and shape.

Deprecated

