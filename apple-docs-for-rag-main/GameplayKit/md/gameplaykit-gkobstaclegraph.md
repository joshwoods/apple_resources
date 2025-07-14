

- GameplayKit
-  GKObstacleGraph 

Class

# GKObstacleGraph

A navigation graph for 2D game worlds that creates a minimal network for precise pathfinding around obstacles.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class GKObstacleGraph where NodeType : GKGraphNode2D
```

## Overview

You create an obstacle graph with a collection of GKObstacle objects. To use the graph for pathfinding, you add GKGraphNode2D objects representing points of interest (such as the current position of a game character and the location it needs to find a route to). Then use methods of the superclass GKGraph to find routes through the graph.

Unlike the related GKMeshGraph class, an obstacle graph creates a minimal network of graph nodes, resulting in paths that are efficient but not smooth.

To learn more about graphs and pathfinding, see Pathfinding in GameplayKit Programming Guide.

## Topics

### Creating a Graph

init(obstacles: [GKPolygonObstacle], bufferRadius: Float, nodeClass: AnyClass)

Initializes a graph with the specified list of obstacles, using the specified node class.

init(obstacles: [GKPolygonObstacle], bufferRadius: Float)

Initializes a graph with the specified list of obstacles.

### Working with Obstacles

var obstacles: [GKPolygonObstacle]

The list of obstacle objects in the graph, each of which describes a polygon-shaped impassable area.

func addObstacles([GKPolygonObstacle])

Adds new obstacles to the graph.

func removeObstacles([GKPolygonObstacle])

Removes the specified obstacle from the graph.

func removeAllObstacles()

Removes all obstacles from the graph.

func nodes(for: GKPolygonObstacle) -> [NodeType]

Returns the group of nodes corresponding to an obstacle in the graph.

### Working with Nodes

func connectUsingObstacles(node: NodeType)

Adds the specified node to the graph, connecting it to its nearest neighbors without creating connections that pass through obstacles or their buffer regions.

func connectUsingObstacles(node: NodeType, ignoring: [GKPolygonObstacle])

Adds the specified node to the graph, connecting it to its nearest neighbors while ignoring the area occupied by the specified obstacles.

func connectUsingObstacles(node: NodeType, ignoringBufferRadiusOf: [GKPolygonObstacle])

Adds the specified node to the graph, connecting it to its nearest neighbors while ignoring the buffer regions around the specified obstacles.

var bufferRadius: Float

The distance from obstacle edges that should also be considered impassable.

### Locking Node Connections

func lockConnection(from: NodeType, to: NodeType)

Prevents the specified nodes from being disconnected due to the addition of obstacles.

func unlockConnection(from: NodeType, to: NodeType)

Allows the specified nodes to be disconnected due to the addition of obstacles.

func isConnectionLocked(from: NodeType, to: NodeType) -> Bool

Returns a Boolean value indicating whether the specified nodes are protected from disconnection due to the addition of obstacles.

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

class GKMeshGraph

A navigation graph for 2D game worlds that creates a space-filling network for smooth pathfinding around obstacles.

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

