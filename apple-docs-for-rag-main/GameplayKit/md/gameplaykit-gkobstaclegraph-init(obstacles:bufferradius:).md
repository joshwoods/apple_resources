

- GameplayKit
- GKObstacleGraph
-  init(obstacles:bufferRadius:) 

Initializer

# init(obstacles:bufferRadius:)

Initializes a graph with the specified list of obstacles.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(
    obstacles: [GKPolygonObstacle],
    bufferRadius: Float
)
```

## Parameters 

`obstacles`  

An array of obstacle objects, each of which describes a polygon-shaped impassable area.

`bufferRadius`  

The distance from obstacle edges that should also be considered impassable.

## Return Value

A new obstacle graph.

## Discussion

This method generates a graph that can be traversed in all directions, except into the areas occupied by obstacles.

Use the `bufferRadius` parameter to take the size of potential travelers into account when determining navigability. For example, if a game character that will use pathfinding has a radius of 20 units (in the same coordinate space you use to define obstacles), specify a buffer radius of 20. As a result, the graph will consider any points within 20 units of an obstacle non-navigable—that is, pathfinding in the graph will not result in any positions that lie inside this buffer region, so you can safely set the character’s center point to the location of a node returned from the findPath(from:to:) method without the character overlapping any obstacles.

This initializer is equivalent to the init(obstacles:bufferRadius:nodeClass:) initializer, but uses the default GKGraphNode2D node class.

## See Also

### Creating a Graph

init(obstacles: [GKPolygonObstacle], bufferRadius: Float, nodeClass: AnyClass)

Initializes a graph with the specified list of obstacles, using the specified node class.

