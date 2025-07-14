

- GameplayKit
- GKGraphNode
-  cost(to:) 

Instance Method

# cost(to:)

Returns the cost to travel from this node to the specified, directly connected, node.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func cost(to node: GKGraphNode) -> Float
```

## Parameters 

`node`  

A node from this node’s connectedNodes list.

## Return Value

The real cost of travel along the specified connection; higher values indicate higher cost.

## Discussion

The GKGraph class uses this method in pathfinding between nodes—the findPath(from:to:) method finds the lowest-cost path between a specified pair of nodes. For the GKGraphNode base class, the cost of travel along any connection is 1, so the findPath(from:to:) method simply counts connections, finding the path that involves traveling through the fewest number of nodes. Because the subclasses GKGraphNode2D and GKGridGraphNode add geometry information to each node, those classes’ implementation of this method calculates the distance between nodes in 2D space, and the findPath(from:to:) method finds the path with the minimum total distance traveled.

Subclasses can implement this method to add other information to the cost. For example, a game might use higher costs to represent travel through regions of a map that are difficult for a character to traverse.

## See Also

### Computing Traversal Costs

func estimatedCost(to: GKGraphNode) -> Float

Returns an underestimate of the cost of travel from this node to the specified node.

