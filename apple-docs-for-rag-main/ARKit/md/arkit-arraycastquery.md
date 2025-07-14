

- ARKit
-  ARRaycastQuery 

Class

# ARRaycastQuery

A mathematical ray you use to find 3D positions on real-world surfaces.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
class ARRaycastQuery
```

## Overview

You create a raycast query by providing a 3D vector and starting place.

To create a raycast query using a 2D screen location and default vector that casts outward in the z-direction from the user, use the convenience functions, makeRaycastQuery(from:allowing:alignment:) on ARView, or raycastQuery(from:allowing:alignment:) on ARSCNView.

Raycasts can intersect with planes (flat surfaces) or meshes (uneven surfaces). To intersect with planes, see ARRaycastQuery.Target. To intersect with meshes, see ARRaycastQuery.Target.estimatedPlane.

## Topics

### Creating a Raycast Query

init(origin: simd_float3, direction: simd_float3, allowing: ARRaycastQuery.Target, alignment: ARRaycastQuery.TargetAlignment)

Creates a new raycast query.

### Specifying the Target

var target: ARRaycastQuery.Target

A plane type that allows the raycast to terminate if it’s encountered.

enum Target

The types of surface you allow a raycast to intersect with.

var targetAlignment: ARRaycastQuery.TargetAlignment

The target’s alignment with respect to gravity.

enum TargetAlignment

A specification that indicates a target’s alignment with respect to gravity

### Interpreting the Ray

var direction: simd_float3

A vector that describes the ray’s trajectory in 3D space.

var origin: simd_float3

A 3D coordinate that defines the ray’s starting place.

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

class ARTrackedRaycast

A raycast query that ARKit repeats in succession to give you refined results over time.

class ARRaycastResult

Information about a real-world surface found by examining a point on the screen.

