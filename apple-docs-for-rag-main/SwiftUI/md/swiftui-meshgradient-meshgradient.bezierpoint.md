

- SwiftUI
- MeshGradient
-  MeshGradient.BezierPoint 

Structure

# MeshGradient.BezierPoint

One location in a gradient mesh, along with the four Bezier control points surrounding it.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@frozen
struct BezierPoint
```

## Topics

### Initializers

init(position: SIMD2&lt;Float>, leadingControlPoint: SIMD2&lt;Float>, topControlPoint: SIMD2&lt;Float>, trailingControlPoint: SIMD2&lt;Float>, bottomControlPoint: SIMD2&lt;Float>)

Creates a new vertex.

### Instance Properties

var bottomControlPoint: SIMD2&lt;Float>

The Bezier control point of the vertex’s bottom edge.

var leadingControlPoint: SIMD2&lt;Float>

The Bezier control point of the vertex’s leading edge.

var position: SIMD2&lt;Float>

The position of the vertex.

var topControlPoint: SIMD2&lt;Float>

The Bezier control point of the vertex’s top edge.

var trailingControlPoint: SIMD2&lt;Float>

The Bezier control point of the vertex’s trailing edge.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- Sendable

