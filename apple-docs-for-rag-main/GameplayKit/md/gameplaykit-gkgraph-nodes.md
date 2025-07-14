

- GameplayKit
- GKGraph
-  nodes 

Instance Property

# nodes

The list of nodes in the graph.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var nodes: [GKGraphNode]? { get }
```

## Discussion

This array can contain nodes that are not connected to other nodes in the graph.

## See Also

### Working with Nodes in a Graph

func add([GKGraphNode])

Adds the specified nodes to the graph.

func connectToLowestCostNode(node: GKGraphNode, bidirectional: Bool)

Adds a node to the graph, connecting it to the node already in the graph for which the connection has the lowest cost.

func remove([GKGraphNode])

Removes the specified nodes from the graph.

