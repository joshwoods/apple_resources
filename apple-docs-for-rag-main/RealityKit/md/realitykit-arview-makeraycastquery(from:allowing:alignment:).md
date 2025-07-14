

- RealityKit
- ARView
-  makeRaycastQuery(from:allowing:alignment:) 

Instance Method

# makeRaycastQuery(from:allowing:alignment:)

Creates a ray-cast query originating from a point in the view, centered on the camera’s field of view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+

``` source
@MainActor @preconcurrency
func makeRaycastQuery(
    from point: CGPoint,
    allowing target: ARRaycastQuery.Target,
    alignment: ARRaycastQuery.TargetAlignment
) -> ARRaycastQuery?
```

## Parameters 

`point`  

A point in the view’s coordinate system.

`target`  

The type of target where the ray should terminate.

`alignment`  

The alignment of the target.

## Return Value

A query result.

## See Also

### Finding entities at a point in the view

func entity(at: CGPoint) -> Entity?

Finds the entity in the AR scene closest to the specified point.

func entities(at: CGPoint) -> [Entity]

Finds the collection of entities at the specified point in the scene.

func hitTest(CGPoint, query: CollisionCastQueryType, mask: CollisionGroup) -> [CollisionCastHit]

Searches for objects corresponding to a point in the view based on a query and a collision mask.

func hitTest(CGPoint, types: ARHitTestResult.ResultType) -> [ARHitTestResult]

Searches for objects corresponding to a point in the view based on a set of result types.

func raycast(from: CGPoint, allowing: ARRaycastQuery.Target, alignment: ARRaycastQuery.TargetAlignment) -> [ARRaycastResult]

Performs a ray cast, where a ray is cast into the scene from the center of the camera through a point in the view, and the results are immediately returned.

func trackedRaycast(from: CGPoint, allowing: ARRaycastQuery.Target, alignment: ARRaycastQuery.TargetAlignment, updateHandler: ([ARRaycastResult]) -> Void) -> ARTrackedRaycast?

Performs a tracked ray cast, where a ray is cast into the scene from the center of the camera through a point in the view.

