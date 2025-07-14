

- ARKit
-  ARHitTestResult Deprecated

Class

# ARHitTestResult

Information about a real-world surface found by examining a point on the screen.

iOS 11.0–14.0DeprecatediPadOS 11.0–14.0DeprecatedMac Catalyst 13.1–14.0Deprecated

``` source
class ARHitTestResult
```

Deprecated

Use raycasting

## Overview

If you use SceneKit or SpriteKit as your renderer, you can search for real-world surfaces at a screen point using:

- ARSCNView hitTest(_:types:)

- ARSKView hitTest(_:types:)

Otherwise, you can search the camera image for real-world content using the ARFrame hitTest(_:types:) method. Because a frame is independent of a view, for this method you pass a point specified in normalized image coordinates (where `(0,0)` is the top left corner of the image and `(1,1)` is the lower right).

All these methods return an array of ARHitTestResult objects describing the content found. The number and order of results in the array depends on the search types you specify and the order you specify them in. For example, consider the code below:

```
let results = view.hitTest(point, [.existingPlaneUsingGeometry, .estimatedHorizontalPlane])
```

This hitTest(_:types:) call searches first for plane anchors already present in the session (according to the session configuration’s planeDetection settings); returning any such results (in order of distance from the camera) as the first elements in the array. This call also (due to the estimatedHorizontalPlane request) attempts to determine whether the hit test ray intersects any horizontal surface not already found by plane detection, and returns that result (if any) as the last element in the array.

## Topics

### Identifying Results

var type: ARHitTestResult.ResultType

The kind of detected feature the search result represents.

struct ResultType

Possible types for specifying a hit-test search, or for the result of a hit-test search.

var anchor: ARAnchor?

The anchor representing the detected surface, if any.

### Examining Result Geometry

var distance: CGFloat

The distance, in meters, from the camera to the detected surface.

var worldTransform: simd_float4x4

The position and orientation of the result relative to the world coordinate system.

var localTransform: simd_float4x4

The position and orientation of the result relative to the nearest anchor or feature point.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

