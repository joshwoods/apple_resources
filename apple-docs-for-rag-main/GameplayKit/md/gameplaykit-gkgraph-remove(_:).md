

- GameplayKit
- GKGraph
-  remove(\_:) 

Instance Method

# remove(\_:)

Removes the specified nodes from the graph.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func remove(_ nodes: [GKGraphNode])
```

## Parameters 

`nodes`  

A node in the graph.

## Discussion

This method has no effect on nodes in the array that are not in the graph.

## See Also

### Working with Nodes in a Graph

func add([GKGraphNode])

Adds the specified nodes to the graph.

func connectToLowestCostNode(node: GKGraphNode, bidirectional: Bool)

Adds a node to the graph, connecting it to the node already in the graph for which the connection has the lowest cost.

var nodes: [GKGraphNode]?

The list of nodes in the graph.

