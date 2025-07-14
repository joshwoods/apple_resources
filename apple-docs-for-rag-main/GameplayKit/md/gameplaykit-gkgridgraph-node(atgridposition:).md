

- GameplayKit
- GKGridGraph
-  node(atGridPosition:) 

Instance Method

# node(atGridPosition:)

Returns the node in the graph at the specified grid coordinates.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func node(atGridPosition position: vector_int2) -> NodeType?
```

## Parameters 

`position`  

The grid location to query.

## Return Value

The grid node at the specified location, or `nil` if there is no node at that location.

## Discussion

This method finds nodes that are part of the grid created by the graph. You can attach other nodes to the graph (for example, to represent the positions of game entities in the grid) with the connectToAdjacentNodes(node:) method, but such nodes are not part of the grid itself.

## See Also

### Working with Nodes

func connectToAdjacentNodes(node: GKGridGraphNode)

Adds the specified node to the graph, connecting it to its nearest neighbors in the grid.

