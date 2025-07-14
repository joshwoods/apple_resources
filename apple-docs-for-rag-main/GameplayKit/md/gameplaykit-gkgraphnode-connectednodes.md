

- GameplayKit
- GKGraphNode
-  connectedNodes 

Instance Property

# connectedNodes

The list of other nodes connected to this node.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var connectedNodes: [GKGraphNode] { get }
```

## Discussion

In GameplayKit, the connections between nodes in a graph are directional. For example, if the connectedNodes list of Node A contains Node B, then a traveler on the graph can move directly from Node A to Node B. For the reverse to also be true, the connectedNodes list of Node B must contain Node A. To conveniently create connections in both directions, use the `bidirectional` parameter of the addConnections(to:bidirectional:) method.

For more information, see GameplayKit Programming Guide.

## See Also

### Working with Connections

func addConnections(to: [GKGraphNode], bidirectional: Bool)

Connects this node to all nodes in the specified list.

func removeConnections(to: [GKGraphNode], bidirectional: Bool)

Removes the connections from this node to the specified nodes.

