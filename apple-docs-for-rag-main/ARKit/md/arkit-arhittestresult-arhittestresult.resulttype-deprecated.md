

- ARKit
- ARHitTestResult
-  ARHitTestResult.ResultType Deprecated

Structure

# ARHitTestResult.ResultType

Possible types for specifying a hit-test search, or for the result of a hit-test search.

iOS 11.0–14.0DeprecatediPadOS 11.0–14.0DeprecatedMac Catalyst 13.1–14.0Deprecated

``` source
struct ResultType
```

Deprecated

Use raycasting

## Topics

### Creating a Result Type

init(rawValue: UInt)

Creates a result type.

### Result Types

static var featurePoint: ARHitTestResult.ResultType

A point on a surface detected by ARKit, but not part of any detected planes.

static var estimatedHorizontalPlane: ARHitTestResult.ResultType

A point on a real-world planar surface detected during the search, whose orientation is perpendicular to gravity.

static var estimatedVerticalPlane: ARHitTestResult.ResultType

A point on a real-world planar surface detected during the search, whose orientation is parallel to gravity.

static var existingPlane: ARHitTestResult.ResultType

A point on a real-world plane (already detected with the planeDetection option), without considering the plane’s size.

static var existingPlaneUsingExtent: ARHitTestResult.ResultType

A point on a real-world plane (already detected with the planeDetection option), respecting the plane’s estimated size.

static var existingPlaneUsingGeometry: ARHitTestResult.ResultType

A point on a real-world plane (already detected with the planeDetection option), respecting the plane’s estimated size and shape.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Identifying Results

var type: ARHitTestResult.ResultType

The kind of detected feature the search result represents.

Deprecated

var anchor: ARAnchor?

The anchor representing the detected surface, if any.

Deprecated

