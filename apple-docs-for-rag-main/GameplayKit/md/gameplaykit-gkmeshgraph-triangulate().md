

- GameplayKit
- GKMeshGraph
-  triangulate() 

Instance Method

# triangulate()

Creates or updates the graph with a network of nodes that describes the open space around its obstacles.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func triangulate()
```

## Discussion

The GKMeshGraph class adds, removes, and arranges nodes to describe the navigable areas around obstacles *only* when you call this method. Typically, you add or remove several obstacles, then call the triangulate() method to update the graph. You should also call this method after changing the triangulationMode property.

After triangulating, the graph reflects the navigability of open space around its obstacles and can be used for any number of findPath(from:to:) calls. Changing the list of obstacles requires retriangulating the graph.

## See Also

### Managing the Mesh

var triangulationMode: GKMeshGraphTriangulationMode

A set of options for how to place graph nodes when triangulating the graph.

func triangle(at: Int) -> GKTriangle

The triangle definition at the specified index.

var triangleCount: Int

The number of triangles in the mesh.

