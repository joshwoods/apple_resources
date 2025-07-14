

- GameplayKit
- GKObstacleGraph
-  obstacles 

Instance Property

# obstacles

The list of obstacle objects in the graph, each of which describes a polygon-shaped impassable area.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var obstacles: [GKPolygonObstacle] { get }
```

## See Also

### Working with Obstacles

func addObstacles([GKPolygonObstacle])

Adds new obstacles to the graph.

func removeObstacles([GKPolygonObstacle])

Removes the specified obstacle from the graph.

func removeAllObstacles()

Removes all obstacles from the graph.

func nodes(for: GKPolygonObstacle) -> [NodeType]

Returns the group of nodes corresponding to an obstacle in the graph.

