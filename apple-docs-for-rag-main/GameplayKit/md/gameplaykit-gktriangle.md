

- GameplayKit
-  GKTriangle 

Structure

# GKTriangle

The definition of a triangle in the mesh, available with the triangle(at:) method.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
struct GKTriangle
```

## Topics

### Initializers

init()

init(points: (vector_float3, vector_float3, vector_float3))

### Instance Properties

var points: (vector_float3, vector_float3, vector_float3)

A set of three points describing the triangle.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Constants

struct GKMeshGraphTriangulationMode

Options for how to place graph nodes when generating the graph, used by the triangulationMode property.

