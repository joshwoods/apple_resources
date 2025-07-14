

- GameplayKit
- GKGraphNode
-  addConnections(to:bidirectional:) 

Instance Method

# addConnections(to:bidirectional:)

Connects this node to all nodes in the specified list.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func addConnections(
    to nodes: [GKGraphNode],
    bidirectional: Bool
)
```

## Parameters 

`nodes`  

The list of nodes to which to form connections.

`bidirectional`  

true to create a connection in both directions; false to create only connections from this node to each of the specified nodes.

## Discussion

In GameplayKit, the connections between nodes in a graph are directional. For example, if the connectedNodes list of Node A contains Node B, then a traveler on the graph can move directly from Node A to Node B. For the reverse to also be true, the connectedNodes list of Node B must contain Node A. Use the `bidirectional` parameter to choose whether to automatically create connections in both directions or create only one-way connections.

## See Also

### Working with Connections

var connectedNodes: [GKGraphNode]

The list of other nodes connected to this node.

func removeConnections(to: [GKGraphNode], bidirectional: Bool)

Removes the connections from this node to the specified nodes.

