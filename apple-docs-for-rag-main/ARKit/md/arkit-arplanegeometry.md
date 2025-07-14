

- ARKit
-  ARPlaneGeometry 

Class

# ARPlaneGeometry

A 3D mesh describing the shape of a detected plane in world-tracking AR sessions.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.1+

``` source
class ARPlaneGeometry
```

## Overview

This class provides the estimated general shape of a detected plane, in the form of a detailed 3D mesh appropriate for use with various rendering technologies or for exporting 3D assets. (For a quick way to visualize a plane geometry using SceneKit, see the ARSCNPlaneGeometry class.)

Unlike the ARPlaneAnchor center and extent properties, which estimate only a rectangular area for a detected plane, a plane anchor’s geometry property provides a more detailed estimate of the 2D area covered by that plane. For example, if ARKit detects a circular tabletop, the resulting ARPlaneGeometry objects roughly match the general shape of the table. As the session continues to run, ARKit provides updated plane anchors whose associated geometry refines the estimated shape of the plane.

You can use this model to more precisely place 3D content that should appear only on a detected flat surface. For example, to ensure that virtual objects don’t fall off the edge of a table. You can also use this model to create occlusion geometry, which hides other virtual content behind the detected surface in the camera image.

The shape of a plane geometry is always convex. That is, the boundary polygon for a plane geometry is a minimal convex hull enclosing all points that ARKit recognizes or estimates are part of the plane.

## Topics

### Accessing Mesh Data

var vertices: [simd_float3]

An array of vertex positions for each point in the plane mesh.

var textureCoordinates: [vector_float2]

An array of texture coordinate values for each point in the plane mesh.

var triangleCount: Int

The number of triangles described by the triangleIndices buffer.

var triangleIndices: [Int16]

An array of indices describing the triangle mesh formed by the plane geometry’s vertex data.

### Finding Boundary Points

var boundaryVertices: [simd_float3]

An array of vertex positions for each point along the plane’s boundary.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Geometry

var geometry: ARPlaneGeometry

A coarse triangle mesh representing the general shape of the detected plane.

class ARSCNPlaneGeometry

A SceneKit representation of the 2D shape of a plane, for use with plane detection results in an AR session.

