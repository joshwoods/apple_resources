

- SwiftUI
- MeshGradient
- MeshGradient.BezierPoint
-  init(position:leadingControlPoint:topControlPoint:trailingControlPoint:bottomControlPoint:) 

Initializer

# init(position:leadingControlPoint:topControlPoint:trailingControlPoint:bottomControlPoint:)

Creates a new vertex.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    position: SIMD2,
    leadingControlPoint: SIMD2,
    topControlPoint: SIMD2,
    trailingControlPoint: SIMD2,
    bottomControlPoint: SIMD2
)
```

## Parameters 

`position`  

The position of the vertex in the coordinate space the gradient is interpreted in.

`leadingControlPoint`  

The Bezier control point of the vertex’s leading edge.

`topControlPoint`  

The Bezier control point of the vertex’s top edge.

`trailingControlPoint`  

The Bezier control point of the vertex’s trailing edge.

`bottomControlPoint`  

The Bezier control point of the vertex’s bottom edge.

