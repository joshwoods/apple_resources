

- ARKit
-  ARRaycastResult 

Class

# ARRaycastResult

Information about a real-world surface found by examining a point on the screen.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
class ARRaycastResult
```

## Overview

If you use ARView or ARSCNView as your renderer, you can search for real-world surfaces at a screen point using the raycast(from:allowing:alignment:), and raycastQuery(from:allowing:alignment:) functions, respectively.

If you use a custom renderer, you can find real-world positions using screen points with:

- The raycastQuery(from:allowing:alignment:) function of ARFrame.

- The raycast(_:) function of ARSession.

For tracked raycasting, you call trackedRaycast(_:updateHandler:) on your app’s current ARSession.

## Topics

### Identifying Results

var worldTransform: simd_float4x4

The position, rotation, and scale, of the ray’s intersection with the target.

var anchor: ARAnchor?

The anchor for the plane that the ray intersected.

var target: ARRaycastQuery.Target

The type of surface that the ray intersects.

enum Target

The types of surface you allow a raycast to intersect with.

var targetAlignment: ARRaycastQuery.TargetAlignment

The alignment of the plane that the ray intersected.

enum TargetAlignment

A specification that indicates a target’s alignment with respect to gravity

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

## See Also

### Raycasting

Placing objects and handling 3D interaction

Place virtual content at tracked, real-world locations, and enable the user to interact with virtual content by using gestures.

class ARRaycastQuery

A mathematical ray you use to find 3D positions on real-world surfaces.

class ARTrackedRaycast

A raycast query that ARKit repeats in succession to give you refined results over time.

