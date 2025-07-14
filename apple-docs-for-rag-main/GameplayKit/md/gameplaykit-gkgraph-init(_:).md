

- GameplayKit
- GKGraph
-  init(\_:) 

Initializer

# init(\_:)

Initializes a graph with the specified list of nodes.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(_ nodes: [GKGraphNode])
```

## Parameters 

`nodes`  

An array of graph node objects—instances of GKGraphNode or of one of its subclasses containing geometry information.

## Return Value

A new graph object.

## Discussion

The nodes in the array need not already be connected—you can connect nodes after adding them to the graph using the connectToLowestCostNode(node:bidirectional:) method on the graph itself or the addConnection:bidirectional: method on individual nodes. Using the findPath(from:to:) method requires connections between nodes.

For more information, see GameplayKit Programming Guide.

