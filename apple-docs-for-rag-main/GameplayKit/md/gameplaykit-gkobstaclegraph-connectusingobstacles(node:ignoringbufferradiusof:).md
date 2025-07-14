

- GameplayKit
- GKObstacleGraph
-  connectUsingObstacles(node:ignoringBufferRadiusOf:) 

Instance Method

# connectUsingObstacles(node:ignoringBufferRadiusOf:)

Adds the specified node to the graph, connecting it to its nearest neighbors while ignoring the buffer regions around the specified obstacles.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func connectUsingObstacles(
    node: NodeType,
    ignoringBufferRadiusOf obstaclesBufferRadiusToIgnore: [GKPolygonObstacle]
)
```

## Parameters 

`node`  

A graph node object containing 2D coordinate information.

`obstaclesBufferRadiusToIgnore`  

An array of obstacles whose buffer regions are to be ignored when adding the node to the graph.

## Discussion

The GKObstacleGraph class automatically maintains a network of nodes that describes the navigable areas around its collection of obstacles. Adding a new node to the graph connects it to these nodes, such that the resulting network can be used to find paths around the obstacles to the position of the new node. GameplayKit adds new connections only if those connections do not represent a path through any obstacles.

Call this method when you need to to connect a node to the graph without taking the buffer regions around certain obstacles into account. Unlike the connectUsingObstacles(node:ignoring:) method, this method still respects the areas encompassed by the specified obstacles. That is, this method does not create a connection to the specified node if that connection passes through any obstacles. This method does, however, create a connection if the specified node lies outside of an obstacle but within that obstacle’s buffer region.

For example, you typically set the bufferRadius property to match the size of the game entities that will use the graph for pathfinding, so that those entities cannot find paths through spaces smaller than themselves. Other game entities might be smaller than that buffer region, however—if the init(obstacles:bufferRadius:) method fails because the target location is outside an obstacle but within that obstacle’s buffer radius, use this method to find a path to that location.

## See Also

### Working with Nodes

func connectUsingObstacles(node: NodeType)

Adds the specified node to the graph, connecting it to its nearest neighbors without creating connections that pass through obstacles or their buffer regions.

func connectUsingObstacles(node: NodeType, ignoring: [GKPolygonObstacle])

Adds the specified node to the graph, connecting it to its nearest neighbors while ignoring the area occupied by the specified obstacles.

var bufferRadius: Float

The distance from obstacle edges that should also be considered impassable.

