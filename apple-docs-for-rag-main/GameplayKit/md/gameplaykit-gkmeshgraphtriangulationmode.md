

- GameplayKit
-  GKMeshGraphTriangulationMode 

Structure

# GKMeshGraphTriangulationMode

Options for how to place graph nodes when generating the graph, used by the triangulationMode property.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
struct GKMeshGraphTriangulationMode
```

## Topics

### Constants

static var vertices: GKMeshGraphTriangulationMode

An option to place graph nodes at each vertex in the generated mesh.

static var centers: GKMeshGraphTriangulationMode

An option to place graph nodes at the center of each polygon in the generated mesh.

static var edgeMidpoints: GKMeshGraphTriangulationMode

An option to place graph nodes at the midpoint of each in the generated mesh.

### Initializers

init(rawValue: UInt)

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

### Constants

struct GKTriangle

The definition of a triangle in the mesh, available with the triangle(at:) method.

