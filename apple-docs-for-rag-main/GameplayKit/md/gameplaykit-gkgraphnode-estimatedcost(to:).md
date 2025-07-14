

- GameplayKit
- GKGraphNode
-  estimatedCost(to:) 

Instance Method

# estimatedCost(to:)

Returns an underestimate of the cost of travel from this node to the specified node.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func estimatedCost(to node: GKGraphNode) -> Float
```

## Parameters 

`node`  

A node connected (directly or indirectly) to this node.

## Return Value

An underestimate of the travel cost to the specified node; higher values indicate higher cost.

## Discussion

The GKGraph class uses this method in pathfinding between nodes—the findPath(from:to:) method finds the lowest-cost path between a specified pair of nodes. (See the cost(to:) method for further discussion.) The pathfinding algorithm involves successive approximation using a heuristic in order to avoid processing too many nodes. The estimatedCost(to:) method provides that heuristic—a quickly computed estimated cost of travel helps the algorithm choose which nodes to process in order to compute the real cost of travel.

The estimated cost must be an *underestimate* of the true cost—that is, in order for the pathfinding algorithm to produce correct results, the heuristic value must not exceed the true cost of travel between nodes. For example, in a 2D graph, the straight-line distance between two distant nodes is an admissible heuristic, because the actual path found will at best be along that line, but might be along a longer path. The subclasses GKGraphNode2D, GKGraphNode3D, and GKGridGraphNode use this approach.

Custom subclasses can implement this method to add game-specific information that might improve the quality of an estimated cost.

## See Also

### Computing Traversal Costs

func cost(to: GKGraphNode) -> Float

Returns the cost to travel from this node to the specified, directly connected, node.

