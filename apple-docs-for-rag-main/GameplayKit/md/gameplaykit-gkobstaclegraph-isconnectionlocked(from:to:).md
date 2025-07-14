

- GameplayKit
- GKObstacleGraph
-  isConnectionLocked(from:to:) 

Instance Method

# isConnectionLocked(from:to:)

Returns a Boolean value indicating whether the specified nodes are protected from disconnection due to the addition of obstacles.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func isConnectionLocked(
    from startNode: NodeType,
    to endNode: NodeType
) -> Bool
```

## Parameters 

`startNode`  

A node in the graph.

`endNode`  

Another node in the graph to which the node `startNode` is directly connected.

## Return Value

true if the connection between the specified nodes has been locked with the lockConnection(from:to:) method; otherwise, false.

## Discussion

By default, adding obstacles with the addObstacles(_:) method disconnects pairs of nodes if the direct path between them intersects an obstacle. This behavior ensures that using the findPathBetweenNodes:toNode: method does not result in a path through the graph that crosses obstacles. With certain nodes, this behavior might not be desirable—use the lockConnection(from:to:) method to protect a connection between nodes from being automatically destroyed and the unlockConnection(from:to:) method to remove such protection.

## See Also

### Locking Node Connections

func lockConnection(from: NodeType, to: NodeType)

Prevents the specified nodes from being disconnected due to the addition of obstacles.

func unlockConnection(from: NodeType, to: NodeType)

Allows the specified nodes to be disconnected due to the addition of obstacles.

