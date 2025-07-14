

- GameplayKit
-  GKGraphNode2D 

Class

# GKGraphNode2D

A node in a navigation graph, associated with a point in continuous 2D space.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class GKGraphNode2D
```

## Overview

Together, a network of nodes form a graph that describes the navigability of a game world. Use graph nodes with a GKGraph, GKObstacleGraph, or GKMeshGraph object to perform actions that relate to the network of nodes as a whole, such as pathfinding to determine routes through the network.

When you use the GKObstacleGraph or GKMeshGraph class to describe a game world in terms of open spaces interrupted by obstacles, GameplayKit automatically creates and manages GKGraphNode2D instances that represent positions along possible paths that navigate around those obstacles.

To learn more about graphs and pathfinding, see Pathfinding in GameplayKit Programming Guide.

## Topics

### Creating a Graph Node

init(point: vector_float2)

Initializes a graph node with the specified point.

class func node(withPoint: vector_float2) -> Self

Creates a graph node with the specified point.

### Inspecting a Node’s Position

var position: vector_float2

The position of the node in continuous 2D space.

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

class GKGraphNode3D

A node in a navigation graph, associated with a point in continuous 3D space.

class GKGridGraphNode

A node in a navigation graph, associated with a position on a discrete two-dimensional grid.

