

- GameplayKit
-  GKGridGraph 

Class

# GKGridGraph

A navigation graph for 2D game worlds where movement is constrained to an integer grid.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class GKGridGraph where NodeType : GKGridGraphNode
```

## Overview

Use this class to generate a graph containing GKGridGraphNode objects representing a specified grid. Then use methods of the superclass GKGraph to find routes through the graph.

To learn more about graphs and pathfinding, see Pathfinding in GameplayKit Programming Guide.

## Topics

### Creating a Graph

init(fromGridStartingAt: vector_int2, width: Int32, height: Int32, diagonalsAllowed: Bool, nodeClass: AnyClass)

Initializes a graph that describes an integer grid with the specified dimensions, using the specified node class.

init(fromGridStartingAt: vector_int2, width: Int32, height: Int32, diagonalsAllowed: Bool)

Initializes a graph that describes an integer grid with the specified dimensions.

### Working with Nodes

func node(atGridPosition: vector_int2) -> NodeType?

Returns the node in the graph at the specified grid coordinates.

func connectToAdjacentNodes(node: GKGridGraphNode)

Adds the specified node to the graph, connecting it to its nearest neighbors in the grid.

### Inspecting a Graph

var diagonalsAllowed: Bool

A Boolean value that indicates whether nodes in the grid are connected to their diagonal neighbors.

var gridOrigin: vector_int2

The lowest x- and y-coordinates that appear in the grid.

var gridWidth: Int

The number of possible x-coordinates in the grid.

var gridHeight: Int

The number of possible y-coordinates in the grid.

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

class GKMeshGraph

A navigation graph for 2D game worlds that creates a space-filling network for smooth pathfinding around obstacles.

class GKGraphNode

A single node in a navigation graph for use in pathfinding.

class GKGraphNode2D

A node in a navigation graph, associated with a point in continuous 2D space.

class GKGraphNode3D

A node in a navigation graph, associated with a point in continuous 3D space.

class GKGridGraphNode

A node in a navigation graph, associated with a position on a discrete two-dimensional grid.

