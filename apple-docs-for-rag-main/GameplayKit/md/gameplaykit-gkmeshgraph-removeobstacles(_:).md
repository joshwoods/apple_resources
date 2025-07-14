

- GameplayKit
- GKMeshGraph
-  removeObstacles(\_:) 

Instance Method

# removeObstacles(\_:)

Removes the specified obstacle from the graph.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func removeObstacles(_ obstacles: [GKPolygonObstacle])
```

## Parameters 

`obstacles`  

An array of obstacle objects to be removed from the graph.

## Discussion

Adding or removing obstacles does not update the graph. The GKMeshGraph class adds, removes, and arranges nodes to describe the navigable areas around obstacles *only* when you call the triangulate() method. Typically, you add or remove several obstacles, then call the triangulate() method to update the graph.

## See Also

### Working with Obstacles

var obstacles: [GKPolygonObstacle]

The list of obstacle objects in the graph, each of which describes a polygon-shaped impassable area.

func addObstacles([GKPolygonObstacle])

Adds new obstacles to the graph.

