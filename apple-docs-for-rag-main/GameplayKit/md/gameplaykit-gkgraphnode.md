

- GameplayKit
-  GKGraphNode 

Class

# GKGraphNode

A single node in a navigation graph for use in pathfinding.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class GKGraphNode
```

## Overview

A set of connected nodes form a graph that describes the navigability of a game world. Use graph nodes together with a GKGraph object (or one of its subclasses) to perform actions that relate to the network of nodes as a whole, such as pathfinding to determine routes through the network.

This class describes the general features of graph nodes, but does not contain geometry information that relates the graph to a game world. You can construct a graph with this class or any of its subclasses:

- On its own, the GKGraphNode class is useful for worlds such as board games, where the connections between nodes are important but their spatial position has no effect on gameplay.

- Create GKGridGraphNode objects (for use with the GKGridGraph class) to model worlds where movement is constrained to a two-dimensional integer grid.

- Create GKGraphNode2D objects to model worlds that allow full freedom of movement in a two-dimensional plane. Use these nodes together with the GKObstacleGraph or GKMeshGraph class to create graphs that route around impassable obstacles.

- Create GKGraphNode3D objects to model worlds that allow full freedom of movement in three-dimensional space.

To learn more about graphs and pathfinding, see Pathfinding in GameplayKit Programming Guide.

## Topics

### Working with Connections

var connectedNodes: [GKGraphNode]

The list of other nodes connected to this node.

func addConnections(to: [GKGraphNode], bidirectional: Bool)

Connects this node to all nodes in the specified list.

func removeConnections(to: [GKGraphNode], bidirectional: Bool)

Removes the connections from this node to the specified nodes.

### Computing Traversal Costs

func cost(to: GKGraphNode) -> Float

Returns the cost to travel from this node to the specified, directly connected, node.

func estimatedCost(to: GKGraphNode) -> Float

Returns an underestimate of the cost of travel from this node to the specified node.

### Finding Paths

func findPath(to: GKGraphNode) -> [GKGraphNode]

Computes and returns a sequence of nodes that represents the lowest-cost graph traversal from this node to the specified node.

func findPath(from: GKGraphNode) -> [GKGraphNode]

Computes and returns a sequence of nodes that represents the lowest-cost graph traversal from the specified node to this node.

## Relationships

### Inherits From

- NSObject

### Inherited By

- GKGraphNode2D
- GKGraphNode3D
- GKGridGraphNode

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Pathfinding

class GKGraph

A collection of nodes that describes the navigability of a game world and provides *pathfinding* methods to search for routes through that space.

class GKObstacleGraph

A navigation graph for 2D game worlds that creates a minimal network for precise pathfinding around obstacles.

class GKMeshGraph

A navigation graph for 2D game worlds that creates a space-filling network for smooth pathfinding around obstacles.

class GKGridGraph

A navigation graph for 2D game worlds where movement is constrained to an integer grid.

class GKGraphNode2D

A node in a navigation graph, associated with a point in continuous 2D space.

class GKGraphNode3D

A node in a navigation graph, associated with a point in continuous 3D space.

class GKGridGraphNode

A node in a navigation graph, associated with a position on a discrete two-dimensional grid.

