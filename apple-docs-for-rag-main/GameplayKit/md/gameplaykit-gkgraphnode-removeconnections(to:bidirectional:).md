

- GameplayKit
- GKGraphNode
-  removeConnections(to:bidirectional:) 

Instance Method

# removeConnections(to:bidirectional:)

Removes the connections from this node to the specified nodes.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func removeConnections(
    to nodes: [GKGraphNode],
    bidirectional: Bool
)
```

## Parameters 

`nodes`  

The nodes connected to this node whose connections are to be removed.

`bidirectional`  

true to remove connections in both directions if they exist; false to remove only connections from this node to each of the specified nodes.

## Discussion

In GameplayKit, the connections between nodes in a graph are directional. For example, if the connectedNodes list of Node A contains Node B, then a traveler on the graph can move directly from Node A to Node B. For the reverse to also be true, the connectedNodes list of Node B must contain Node A. When calling this method to remove a connection from one node to another, use the `bidirectional` parameter to choose whether to automatically remove the reverse connection as well.

## See Also

### Working with Connections

var connectedNodes: [GKGraphNode]

The list of other nodes connected to this node.

func addConnections(to: [GKGraphNode], bidirectional: Bool)

Connects this node to all nodes in the specified list.

