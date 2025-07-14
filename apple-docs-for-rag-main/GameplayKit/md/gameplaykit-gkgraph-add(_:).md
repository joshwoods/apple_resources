

- GameplayKit
- GKGraph
-  add(\_:) 

Instance Method

# add(\_:)

Adds the specified nodes to the graph.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func add(_ nodes: [GKGraphNode])
```

## Parameters 

`nodes`  

An array of graph node objects—instances of GKGraphNode or of one of its subclasses that adds geometry information.

## Discussion

Calling this method does not connect the newly added nodes to others in the graph.

## See Also

### Working with Nodes in a Graph

func connectToLowestCostNode(node: GKGraphNode, bidirectional: Bool)

Adds a node to the graph, connecting it to the node already in the graph for which the connection has the lowest cost.

func remove([GKGraphNode])

Removes the specified nodes from the graph.

var nodes: [GKGraphNode]?

The list of nodes in the graph.

