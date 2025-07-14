

- GameplayKit
- GKObstacleGraph
-  removeObstacles(\_:) 

Instance Method

# removeObstacles(\_:)

Removes the specified obstacle from the graph.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func removeObstacles(_ obstacles: [GKPolygonObstacle])
```

## Parameters 

`obstacles`  

An array of obstacle objects to be removed from the graph.

## Discussion

After removing obstacles, the GKObstacleGraph class automatically creates, removes, or rearranges nodes and edges where necessary to describe the navigable area around the complete collection of obstacles.

## See Also

### Working with Obstacles

var obstacles: [GKPolygonObstacle]

The list of obstacle objects in the graph, each of which describes a polygon-shaped impassable area.

func addObstacles([GKPolygonObstacle])

Adds new obstacles to the graph.

func removeAllObstacles()

Removes all obstacles from the graph.

func nodes(for: GKPolygonObstacle) -> [NodeType]

Returns the group of nodes corresponding to an obstacle in the graph.

