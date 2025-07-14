

- GameplayKit
- GKObstacleGraph
-  init(obstacles:bufferRadius:nodeClass:) 

Initializer

# init(obstacles:bufferRadius:nodeClass:)

Initializes a graph with the specified list of obstacles, using the specified node class.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(
    obstacles: [GKPolygonObstacle],
    bufferRadius: Float,
    nodeClass: AnyClass
)
```

## Parameters 

`obstacles`  

An array of obstacle objects, each of which describes a polygon-shaped impassable area.

`bufferRadius`  

The distance from obstacle edges that should also be considered impassable.

`nodeClass`  

The GKGraphNode2D subclass to use for nodes in the graph.

## Return Value

A new obstacle graph.

## Discussion

This method generates a graph that can be traversed in all directions, except into the areas occupied by obstacles.

Use the `bufferRadius` parameter to take the size of potential travelers into account when determining navigability. For example, if a game character that will use pathfinding has a radius of 20 units (in the same coordinate space you use to define obstacles), specify a buffer radius of 20. As a result, the graph will consider any points within 20 units of an obstacle non-navigable—that is, pathfinding in the graph will not result in any positions that lie inside this buffer region, so you can safely set the character’s center point to the location of a node returned from the findPath(from:to:) method without the character overlapping any obstacles.

Use the `nodeClass` parameter to create a graph using a custom subclass of GKGraphNode2D. For example, your custom node class might override the cost(to:) method so that some nodes are more costly than others to travel through. Pathfinding in such a graph would favor indirect routes when a direct route has a higher cost.

For more information, see GameplayKit Programming Guide.

## See Also

### Creating a Graph

init(obstacles: [GKPolygonObstacle], bufferRadius: Float)

Initializes a graph with the specified list of obstacles.

