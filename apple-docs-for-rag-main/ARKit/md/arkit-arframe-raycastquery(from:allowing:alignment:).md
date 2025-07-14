

- ARKit
- ARFrame
-  raycastQuery(from:allowing:alignment:) 

Instance Method

# raycastQuery(from:allowing:alignment:)

Get a ray-cast query for a screen point.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func raycastQuery(
    from point: CGPoint,
    allowing target: ARRaycastQuery.Target,
    alignment: ARRaycastQuery.TargetAlignment
) -> ARRaycastQuery
```

## Parameters 

`point`  

A normalized coordinate in the UI system, where 0 is top-left, and 1 is bottom-right.

`target`  

The types of plane you allow this ray cast to intersect with.

`alignment`  

An alignment with respect to gravity a plane must have to interset this ray.

## Discussion

To cast the ray, you pass the resulting query to your current session via raycast(_:) or trackedRaycast(_:updateHandler:).

## See Also

### Tracking and interacting with the real world

var anchors: [ARAnchor]

The list of anchors representing positions tracked or objects detected in the scene.

func hitTest(CGPoint, types: ARHitTestResult.ResultType) -> [ARHitTestResult]

Searches for real-world objects or AR anchors in the captured camera image.

Deprecated

