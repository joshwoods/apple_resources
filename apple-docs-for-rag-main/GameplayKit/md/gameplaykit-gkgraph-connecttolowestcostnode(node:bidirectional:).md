

- GameplayKit
- GKGraph
-  connectToLowestCostNode(node:bidirectional:) 

Instance Method

# connectToLowestCostNode(node:bidirectional:)

Adds a node to the graph, connecting it to the node already in the graph for which the connection has the lowest cost.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func connectToLowestCostNode(
    node: GKGraphNode,
    bidirectional: Bool
)
```

## Parameters 

`node`  

A graph node object.

`bidirectional`  

true to create connections in both directions; false to create just a single connection from the nearest node to the newly added node.

## Discussion

This method uses the cost(to:) method of the specified node to find the node already in the graph that is most easily reached from the new node. For nodes that contain geometry information (GKGraphNode2D or GKGridGraphNode objects), cost is by default based on distance, so this method connects the new node to the geometrically closest node already in the graph. If you create a custom GKGraphNode subclass, this method selects the “closest” node according to whatever algorithm you implement in your cost(to:) method.

Using this method with an instance of the GKGraphNode base class is not recommended.

## See Also

### Working with Nodes in a Graph

func add([GKGraphNode])

Adds the specified nodes to the graph.

func remove([GKGraphNode])

Removes the specified nodes from the graph.

var nodes: [GKGraphNode]?

The list of nodes in the graph.

