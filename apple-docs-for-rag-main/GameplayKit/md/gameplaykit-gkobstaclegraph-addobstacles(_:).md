

- GameplayKit
- GKObstacleGraph
-  addObstacles(\_:) 

Instance Method

# addObstacles(\_:)

Adds new obstacles to the graph.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func addObstacles(_ obstacles: [GKPolygonObstacle])
```

## Parameters 

`obstacles`  

An array of obstacle objects to be added to the graph.

## Discussion

Adding a new obstacle to the graph has the same effect as if that obstacle were present when creating the graph—that is, the GKObstacleGraph class automatically creates new nodes and edges where necessary to describe the navigable area around the complete collection of obstacles.

## See Also

### Working with Obstacles

var obstacles: [GKPolygonObstacle]

The list of obstacle objects in the graph, each of which describes a polygon-shaped impassable area.

func removeObstacles([GKPolygonObstacle])

Removes the specified obstacle from the graph.

func removeAllObstacles()

Removes all obstacles from the graph.

func nodes(for: GKPolygonObstacle) -> [NodeType]

Returns the group of nodes corresponding to an obstacle in the graph.

