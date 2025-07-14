

- GameplayKit
- GKMeshGraph
-  triangleCount 

Instance Property

# triangleCount

The number of triangles in the mesh.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var triangleCount: Int { get }
```

## Discussion

This property’s value is valid only after calling the triangulate() to create a mesh around the current configuration of obstacles.

## See Also

### Managing the Mesh

func triangulate()

Creates or updates the graph with a network of nodes that describes the open space around its obstacles.

var triangulationMode: GKMeshGraphTriangulationMode

A set of options for how to place graph nodes when triangulating the graph.

func triangle(at: Int) -> GKTriangle

The triangle definition at the specified index.

