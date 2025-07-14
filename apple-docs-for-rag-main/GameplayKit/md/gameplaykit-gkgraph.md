

- GameplayKit
-  GKGraph 

Class

# GKGraph

A collection of nodes that describes the navigability of a game world and provides *pathfinding* methods to search for routes through that space.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class GKGraph
```

## Overview

Individual nodes in a graph represent discrete locations that a character or other object in your game can occupy, and the connections between adjacent nodes represent the ability of a game entity to travel from one location to another. Use the GKGraph class to create a general graph, or the GKGridGraph, GKObstacleGraph, or GKMeshGraph subclass to generate specialized graphs that contain more information about the geometry of your game world.

Each set of graph and node classes can generate graphs for different kinds of spaces:

- The base classes GKGraph and GKGraphNode contain functionality general to all graphs and nodes. You can also use these classes on their own to construct graphs that contain no geometry information. This option is useful for games where the connections between spaces are more important than their physical locations, such as board games.

- Use the GKGridGraph and GKGridGraphNode classes to describe game worlds that constrain movement to an integer grid, such as tactical role-playing games.

- Use the GKObstacleGraph or GKMeshGraph class to describe 2D game worlds that allow continuous movement in open spaces that are interrupted by impassable obstacles (GKPolygonObstacle objects). Obstacle graphs automatically generate nodes containing 2D point information (GKGraphNode2D objects), and you can also add your own such nodes representing locations of interest.

The graphs modeled by this class are always *directed*—that is, a connection between two nodes describes one direction of travel between them. To enable travel between two nodes in either direction, you must create a connection in each direction. You can choose to connect both directions at once with the connectToLowestCostNode(node:bidirectional:) method (for graphs) or the addConnection:bidirectional: method (for nodes).

Using a graph for pathfinding typically involves three major steps:

1.  Create a graph once (for example, when initializing a game level class) with static information about your game world.

2.  When you need to find a route between points, connect temporary nodes to the graph at those points. Use the connectToLowestCostNode(node:bidirectional:) method to connect nodes using their own geometry information, or the connectUsingObstacles(node:) or connectToAdjacentNodes(node:) method to use the additional constraints of obstacle and grid graphs.

3.  Call the findPath(from:to:) method to find a route between locations in the graph. This method returns an array of graph nodes, starting with the requested start point of the path, and proceeding to adjacent nodes in order until it reaches the requested end point. Use the geometry information contained in each node to make use of the route—for example, in a SpriteKit game you might create a sequence of move actions to move a character from point to point along the path.

4.  The temporary nodes you created for finding a path typically have little usefulness after a path has been found. Remove those nodes before reusing the graph for future searches.

To learn more about graphs and pathfinding, see Pathfinding in GameplayKit Programming Guide.

## Topics

### Creating a Graph

init([GKGraphNode])

Initializes a graph with the specified list of nodes.

### Working with Nodes in a Graph

func add([GKGraphNode])

Adds the specified nodes to the graph.

func connectToLowestCostNode(node: GKGraphNode, bidirectional: Bool)

Adds a node to the graph, connecting it to the node already in the graph for which the connection has the lowest cost.

func remove([GKGraphNode])

Removes the specified nodes from the graph.

var nodes: [GKGraphNode]?

The list of nodes in the graph.

### Pathfinding with a Graph

func findPath(from: GKGraphNode, to: GKGraphNode) -> [GKGraphNode]

Computes and returns a sequence of nodes that represents the shortest traversal of the graph between the specified nodes.

## Relationships

### Inherits From

- NSObject

### Inherited By

- GKGridGraph
- GKMeshGraph
- GKObstacleGraph

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

class GKObstacleGraph

A navigation graph for 2D game worlds that creates a minimal network for precise pathfinding around obstacles.

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

