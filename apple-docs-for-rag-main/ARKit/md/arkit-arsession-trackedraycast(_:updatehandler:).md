

- ARKit
- ARSession
-  trackedRaycast(\_:updateHandler:) 

Instance Method

# trackedRaycast(\_:updateHandler:)

Repeats a ray-cast query over time to notify you of updated surfaces in the physical environment.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func trackedRaycast(
    _ query: ARRaycastQuery,
    updateHandler: @escaping ([ARRaycastResult]) -> Void
) -> ARTrackedRaycast?
```

## Parameters 

`query`  

The ray-cast query that ARKit will repeat. If you use a standard renderer, you ask the standard renderer to provide the ray-cast query; see Finding Real-World Surfaces of ARSCNView. If you use a custom renderer, you create a ray-cast query by specifying a point on a particular frame; see `Finding Real-World Surfaces` in ARFrame.

`updateHandler`  

A closure you provide that ARKit calls every time it has an updated ray-cast result for you. Use this opportunity to update the position of any virtual content your app may have placed using the prior results of the tracked ray cast. ARKit invokes this closure on your session’s delegate queue.

## Discussion

A tracked ray cast wraps a ray-cast query that the session calls repeatedly, each time invoking your update handler to provide you with new results.

When you’re ready to stop a tracked ray cast, call stopTracking().

## See Also

### Finding real-world surfaces

func raycast(ARRaycastQuery) -> [ARRaycastResult]

Checks once for intersections between a ray and real-world surfaces.

