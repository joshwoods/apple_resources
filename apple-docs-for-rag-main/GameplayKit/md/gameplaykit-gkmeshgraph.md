

- GameplayKit
-  GKMeshGraph 

Class

# GKMeshGraph

A navigation graph for 2D game worlds that creates a space-filling network for smooth pathfinding around obstacles.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
class GKMeshGraph where NodeType : GKGraphNode2D
```

## Overview

To use a mesh graph for pathfinding, add a collection of GKObstacle objects representing impassable areas and GKGraphNode2D objects representing points of interest (such as the current position of a game character and the location it needs to find a route to). Then use methods of the superclass GKGraph to find routes through the graph.

Unlike the related GKObstacleGraph class, a mesh graph creates a space-filling network of graph nodes, resulting in paths that are smooth but not the most efficient.

To learn more about graphs and pathfinding, see Pathfinding in GameplayKit Programming Guide.

## Topics

### Creating a Graph

init(bufferRadius: Float, minCoordinate: vector_float2, maxCoordinate: vector_float2, nodeClass: AnyClass)

Initializes a graph to cover the specified area, using the specified node class.

init(bufferRadius: Float, minCoordinate: vector_float2, maxCoordinate: vector_float2)

Initializes a graph to cover the specified area.

### Working with Obstacles

var obstacles: [GKPolygonObstacle]

The list of obstacle objects in the graph, each of which describes a polygon-shaped impassable area.

func addObstacles([GKPolygonObstacle])

Adds new obstacles to the graph.

func removeObstacles([GKPolygonObstacle])

Removes the specified obstacle from the graph.

### Working with Nodes

func connectUsingObstacles(node: NodeType)

Adds the specified node to the graph, connecting it to its nearest neighbors without creating connections that pass through obstacles or their buffer regions.

var bufferRadius: Float

The distance from obstacle edges that should also be considered impassable.

### Managing the Mesh

func triangulate()

Creates or updates the graph with a network of nodes that describes the open space around its obstacles.

var triangulationMode: GKMeshGraphTriangulationMode

A set of options for how to place graph nodes when triangulating the graph.

func triangle(at: Int) -> GKTriangle

The triangle definition at the specified index.

var triangleCount: Int

The number of triangles in the mesh.

### Constants

struct GKMeshGraphTriangulationMode

Options for how to place graph nodes when generating the graph, used by the triangulationMode property.

struct GKTriangle

The definition of a triangle in the mesh, available with the triangle(at:) method.

### Instance Methods

func classForGenericArgument(at: Int) -> AnyClass

## Relationships

### Inherits From

- GKGraph

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Pathfinding

class GKGraph

A collection of nodes that describes the navigability of a game world and provides *pathfinding* methods to search for routes through that space.

class GKObstacleGraph

A navigation graph for 2D game worlds that creates a minimal network for precise pathfinding around obstacles.

class GKGridGraph

A navigation graph for 2D game worlds where movement is constrained to an integer grid.

class GKGraphNode

A single node in a navigation graph for use in pathfinding.

class GKGraphNode2D

A node in a navigation graph, associated with a point in continuous 2D space.

class GKGraphNode3D

A node in a navigation graph, associated with a point in continuous 3D space.

class GKGridGraphNode

A node in a navigation graph, associated with a position on a discrete two-dimensional grid.

