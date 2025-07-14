

- ARKit
- ARSession
-  raycast(\_:) 

Instance Method

# raycast(\_:)

Checks once for intersections between a ray and real-world surfaces.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func raycast(_ query: ARRaycastQuery) -> [ARRaycastResult]
```

## Parameters 

`query`  

The ray you create from a screen point you’re interested in.

## Return Value

An array of ray-cast results, sorted from nearest to furthest from the camera. The array is empty if the ray cast fails to find an intersection between the query’s ray and a real-world surface.

## Discussion

Ray casting provides a 3D location in physical space that corresponds to a given 2D location on the screen. When you call this function, it succeeds in returning a result when a mathematical ray that ARKit casts outward from the user intersects with any real-world surfaces that ARKit detects in the physical environment.

## See Also

### Finding real-world surfaces

func trackedRaycast(ARRaycastQuery, updateHandler: ([ARRaycastResult]) -> Void) -> ARTrackedRaycast?

Repeats a ray-cast query over time to notify you of updated surfaces in the physical environment.

