

- GameplayKit
-  GKGraphNode3D 

Class

# GKGraphNode3D

A node in a navigation graph, associated with a point in continuous 3D space.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
class GKGraphNode3D
```

## Overview

Together, a network of nodes form a graph that describes the navigability of a game world. Use graph nodes with a GKGraph object to perform actions that relate to the network of nodes as a whole, such as pathfinding to determine routes through the network.

To learn more about graphs and pathfinding, see Pathfinding in GameplayKit Programming Guide.

## Topics

### Creating a Graph Node

init(point: vector_float3)

Initializes a graph node with the specified point.

class func node(withPoint: vector_float3) -> Self

Creates a graph node with the specified point.

### Inspecting a Node’s Position

var position: vector_float3

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

class GKGraphNode2D

A node in a navigation graph, associated with a point in continuous 2D space.

class GKGridGraphNode

A node in a navigation graph, associated with a position on a discrete two-dimensional grid.

