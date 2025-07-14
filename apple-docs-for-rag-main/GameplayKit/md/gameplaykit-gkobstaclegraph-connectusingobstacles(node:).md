

- GameplayKit
- GKObstacleGraph
-  connectUsingObstacles(node:) 

Instance Method

# connectUsingObstacles(node:)

Adds the specified node to the graph, connecting it to its nearest neighbors without creating connections that pass through obstacles or their buffer regions.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func connectUsingObstacles(node: NodeType)
```

## Parameters 

`node`  

A graph node object containing 2D coordinate information.

## Discussion

The GKObstacleGraph class automatically maintains a network of nodes that describes the navigable areas around its collection of obstacles. Adding a new node to the graph connects it to these nodes, such that the resulting network can be used to find paths around the obstacles to the position of the new node. GameplayKit adds new connections only if those connections do not represent a path through any obstacles (or through the buffer region around them, as specified by the bufferRadius property.)

Calling this method is equivalent to calling the connectUsingObstacles(node:ignoring:) and passing an empty array for the `obstaclesToIgnore` parameter.

## See Also

### Working with Nodes

func connectUsingObstacles(node: NodeType, ignoring: [GKPolygonObstacle])

Adds the specified node to the graph, connecting it to its nearest neighbors while ignoring the area occupied by the specified obstacles.

func connectUsingObstacles(node: NodeType, ignoringBufferRadiusOf: [GKPolygonObstacle])

Adds the specified node to the graph, connecting it to its nearest neighbors while ignoring the buffer regions around the specified obstacles.

var bufferRadius: Float

The distance from obstacle edges that should also be considered impassable.

