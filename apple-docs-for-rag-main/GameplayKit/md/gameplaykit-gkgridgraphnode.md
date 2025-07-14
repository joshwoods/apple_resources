

- GameplayKit
-  GKGridGraphNode 

Class

# GKGridGraphNode

A node in a navigation graph, associated with a position on a discrete two-dimensional grid.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class GKGridGraphNode
```

## Overview

Together, a network of nodes form a graph that describes the navigability of a game world. Use graph nodes with a GKGridGraph object (and methods of its superclass GKGraph) to perform actions that relate to the network of nodes as a whole, such as pathfinding to determine routes through the network.

To learn more about graphs and pathfinding, see Pathfinding in GameplayKit Programming Guide.

## Topics

### Creating a Graph Node

init(gridPosition: vector_int2)

Initializes a graph node with the specified position on a grid.

### Inspecting a Node’s Position

var gridPosition: vector_int2

The position of the node on a discrete integer grid.

## Relationships

### Inherits From

- GKGraphNode

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

class GKGraphNode

A single node in a navigation graph for use in pathfinding.

class GKGraphNode2D

A node in a navigation graph, associated with a point in continuous 2D space.

class GKGraphNode3D

A node in a navigation graph, associated with a point in continuous 3D space.

