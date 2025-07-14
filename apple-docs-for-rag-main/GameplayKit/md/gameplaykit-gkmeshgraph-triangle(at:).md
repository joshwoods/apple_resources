

- GameplayKit
- GKMeshGraph
-  triangle(at:) 

Instance Method

# triangle(at:)

The triangle definition at the specified index.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func triangle(at index: Int) -> GKTriangle
```

## Parameters 

`index`  

An index identifying the triangle. Must be less than the value of the triangleCount property.

## Return Value

A structure describing the specified triangle.

## Discussion

This method provides valid results only after calling the triangulate() to create a mesh around the current configuration of obstacles. The information this method provides can be useful for drawing your own overlay UI to debug the graphs you create.

## See Also

### Managing the Mesh

func triangulate()

Creates or updates the graph with a network of nodes that describes the open space around its obstacles.

var triangulationMode: GKMeshGraphTriangulationMode

A set of options for how to place graph nodes when triangulating the graph.

var triangleCount: Int

The number of triangles in the mesh.

