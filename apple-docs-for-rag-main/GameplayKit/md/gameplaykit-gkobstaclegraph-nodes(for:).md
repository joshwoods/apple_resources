

- GameplayKit
- GKObstacleGraph
-  nodes(for:) 

Instance Method

# nodes(for:)

Returns the group of nodes corresponding to an obstacle in the graph.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func nodes(for obstacle: GKPolygonObstacle) -> [NodeType]
```

## Parameters 

`obstacle`  

An obstacle in the graph.

## Return Value

An array of nodes representing the navigable points nearest to each of the obstacle’s vertices.

## Discussion

Adding obstacles to a graph creates additional graph nodes corresponding to the navigable points nearest to each of the obstacle’s vertices. The GKObstacleGraph class automatically creates, removes, or rearranges these nodes where necessary, and automatically connects or disconnects other nodes so that no path between nodes passes through an obstacle.

## See Also

### Working with Obstacles

var obstacles: [GKPolygonObstacle]

The list of obstacle objects in the graph, each of which describes a polygon-shaped impassable area.

func addObstacles([GKPolygonObstacle])

Adds new obstacles to the graph.

func removeObstacles([GKPolygonObstacle])

Removes the specified obstacle from the graph.

func removeAllObstacles()

Removes all obstacles from the graph.

