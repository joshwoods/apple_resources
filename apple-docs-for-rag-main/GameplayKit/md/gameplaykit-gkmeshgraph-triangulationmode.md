

- GameplayKit
- GKMeshGraph
-  triangulationMode 

Instance Property

# triangulationMode

A set of options for how to place graph nodes when triangulating the graph.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var triangulationMode: GKMeshGraphTriangulationMode { get set }
```

## Discussion

The triangulate() method creates an internal model the empty space around the obstacles in the graph in the form of a polygon mesh. The mesh is generated such that the empty space divides into roughly even partitions, each of which is no more than a certain distance from an obstacle. After generating the mesh, the triangulate() method adds nodes to the graph corresponding to locations in the mesh. This property controls which locations in the mesh become nodes in the graph.

The GKMeshGraphTriangulationMode type is an option set: you can place nodes using multiple modes by combining the relevant constants with OptionSet syntax, or bitwise OR operations in Objective-C. Combining modes yields a denser graph, which can lead to slower pathfinding operations but smoother resulting paths. For best results, experiment with different modes and combinations to find the most natural style of movement for your game.

## See Also

### Managing the Mesh

func triangulate()

Creates or updates the graph with a network of nodes that describes the open space around its obstacles.

func triangle(at: Int) -> GKTriangle

The triangle definition at the specified index.

var triangleCount: Int

The number of triangles in the mesh.

