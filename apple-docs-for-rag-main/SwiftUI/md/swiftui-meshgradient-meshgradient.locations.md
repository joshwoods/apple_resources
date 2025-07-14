

- SwiftUI
- MeshGradient
-  MeshGradient.Locations 

Enumeration

# MeshGradient.Locations

An array of 2D locations and their control points.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
enum Locations
```

## Topics

### Enumeration Cases

case bezierPoints([MeshGradient.BezierPoint])

Vertices explicitly specifying their location and control points.

case points([SIMD2&lt;Float>])

Vertices are only specified as their location, their control points are inferred from the locations of their neighbors.

## Relationships

### Conforms To

- Equatable
- Sendable

