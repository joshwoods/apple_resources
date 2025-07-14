

- GameplayKit
- GKMeshGraph
-  obstacles 

Instance Property

# obstacles

The list of obstacle objects in the graph, each of which describes a polygon-shaped impassable area.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var obstacles: [GKPolygonObstacle] { get }
```

## See Also

### Working with Obstacles

func addObstacles([GKPolygonObstacle])

Adds new obstacles to the graph.

func removeObstacles([GKPolygonObstacle])

Removes the specified obstacle from the graph.

