

- GameplayKit
- GKGridGraph
-  connectToAdjacentNodes(node:) 

Instance Method

# connectToAdjacentNodes(node:)

Adds the specified node to the graph, connecting it to its nearest neighbors in the grid.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func connectToAdjacentNodes(node: GKGridGraphNode)
```

## Parameters 

`node`  

A graph node object containing integer grid coordinate information.

## Discussion

Nodes attached through this method do not become part of the grid itself, but instead can represent positions of game entities in the grid. Use nodes connected in this way to find paths between such positions.

## See Also

### Working with Nodes

func node(atGridPosition: vector_int2) -> NodeType?

Returns the node in the graph at the specified grid coordinates.

