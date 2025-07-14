

- ARKit
- ARFrame
-  hitTest(\_:types:) Deprecated

Instance Method

# hitTest(\_:types:)

Searches for real-world objects or AR anchors in the captured camera image.

iOS 11.0–14.0DeprecatediPadOS 11.0–14.0DeprecatedMac Catalyst 13.1–14.0Deprecated

``` source
func hitTest(
    _ point: CGPoint,
    types: ARHitTestResult.ResultType
) -> [ARHitTestResult]
```

Deprecated

Use \[ARSession raycast:\]

## Parameters 

`point`  

A point in normalized image coordinate space. (The point `(0,0)` represents the top left corner of the image, and the point `(1,1)` represents the bottom right corner.)

`types`  

The types of hit-test result to search for.

## Return Value

A list of results, sorted from nearest to farthest (in distance from the camera).

## Mentioned in 

Displaying an AR Experience with Metal

## Discussion

Hit testing searches for real-world objects or surfaces detected through the AR session’s processing of the camera image. A 2D point in the image coordinates can refer to any point along a 3D line that starts at the device camera and extends in a direction determined by the device orientation and camera projection. This method searches along that line, returning all objects that intersect it in order of distance from the camera.

Note

If you use ARKit with a SceneKit or SpriteKit view, the ARSCNView hitTest(_:types:) or ARSKView hitTest(_:types:) method lets you specify a search point in view coordinates.

The behavior of a hit test depends on which `types` you specify and the order you specify them in. For details, see ARHitTestResult and the various ARHitTestResult.ResultType options.

## See Also

### Tracking and interacting with the real world

var anchors: [ARAnchor]

The list of anchors representing positions tracked or objects detected in the scene.

func raycastQuery(from: CGPoint, allowing: ARRaycastQuery.Target, alignment: ARRaycastQuery.TargetAlignment) -> ARRaycastQuery

Get a ray-cast query for a screen point.

