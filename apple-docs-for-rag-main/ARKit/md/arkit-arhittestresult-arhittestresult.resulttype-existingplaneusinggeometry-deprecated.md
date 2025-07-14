

- ARKit
- ARHitTestResult
- ARHitTestResult.ResultType
-  existingPlaneUsingGeometry Deprecated

Type Property

# existingPlaneUsingGeometry

A point on a real-world plane (already detected with the planeDetection option), respecting the plane’s estimated size and shape.

iOS 11.3–14.0DeprecatediPadOS 11.3–14.0DeprecatedMac Catalyst 13.1–14.0Deprecated

``` source
static var existingPlaneUsingGeometry: ARHitTestResult.ResultType { get }
```

## Discussion

When searching for this result type, ARKit returns a point coplanar with an already detected plane only if that point lies within the area defined by the plane’s geometry. That property (together with the anchor’s transform) defines the smallest polygonal area that includes all regions ARKit estimates to be a part of the plane.

Because that polygon is always convex, it may contain regions that are not part of the same real-world surface. (It does, however, provide a more precise esitmate than a bounding rectangle provided by the existingPlaneUsingExtent type.) There may also be parts of the same real-world surface that lie outside the polygon because ARKit has not yet recognized them as part of the same plane. You extend your hit test to an infinite plane by using the existingPlane type.

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

static var existingPlaneUsingExtent: ARHitTestResult.ResultType

A point on a real-world plane (already detected with the planeDetection option), respecting the plane’s estimated size.

Deprecated

