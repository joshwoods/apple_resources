

- GameplayKit
- GKObstacleGraph
-  connectUsingObstacles(node:ignoring:) 

Instance Method

# connectUsingObstacles(node:ignoring:)

Adds the specified node to the graph, connecting it to its nearest neighbors while ignoring the area occupied by the specified obstacles.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func connectUsingObstacles(
    node: NodeType,
    ignoring obstaclesToIgnore: [GKPolygonObstacle]
)
```

## Parameters 

`node`  

A graph node object containing 2D coordinate information.

`obstaclesToIgnore`  

An array of obstacles to be ignored when adding the node to the graph.

## Discussion

The GKObstacleGraph class automatically maintains a network of nodes that describes the navigable areas around its collection of obstacles. Adding a new node to the graph connects it to these nodes, such that the resulting network can be used to find paths around the obstacles to the position of the new node. GameplayKit adds new connections only if those connections do not represent a path through any obstacles (or through the buffer region around them, as specified by the bufferRadius property.)

Call this method when you need to to connect a node to the graph without taking certain obstacles into account. For example, you might add a node representing the destination for a game character to move toward, but place that node inside an existing obstacle, so that the resulting path gets the character as near to that obstacle as possible.

## See Also

### Working with Nodes

func connectUsingObstacles(node: NodeType)

Adds the specified node to the graph, connecting it to its nearest neighbors without creating connections that pass through obstacles or their buffer regions.

func connectUsingObstacles(node: NodeType, ignoringBufferRadiusOf: [GKPolygonObstacle])

Adds the specified node to the graph, connecting it to its nearest neighbors while ignoring the buffer regions around the specified obstacles.

var bufferRadius: Float

The distance from obstacle edges that should also be considered impassable.

