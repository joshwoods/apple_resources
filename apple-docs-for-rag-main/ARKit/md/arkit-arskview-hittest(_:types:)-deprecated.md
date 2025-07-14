

- ARKit
- ARSKView
-  hitTest(\_:types:) Deprecated

Instance Method

# hitTest(\_:types:)

Searches for real-world objects or AR anchors in the captured camera image corresponding to a point in the SpriteKit view.

iOS 11.0–14.0DeprecatediPadOS 11.0–14.0DeprecatedMac Catalyst 13.1–14.0Deprecated

``` source
@MainActor
func hitTest(
    _ point: CGPoint,
    types: ARHitTestResult.ResultType
) -> [ARHitTestResult]
```

Deprecated

Use raycasting

## Parameters 

`point`  

A point in the 2D coordinate system of the view.

`types`  

The types of hit-test result to search for.

## Return Value

A list of results, sorted from nearest to farthest (in distance from the camera).

## Discussion

Hit testing searches for real-world objects or surfaces detected through the AR session’s processing of the camera image. A 2D point in the view’s coordinate system can refer to any point along a 3D line that starts at the device camera and extends in a direction determined by the device orientation and camera projection. This method searches along that line, returning all objects that intersect it in order of distance from the camera.

Note

This method searches for AR anchors and real-world objects detected by the AR session, not SpriteKit content displayed in the view. To search for SpriteKit objects, use the nodes(at:) method of the view’s SpriteKit scene.

The behavior of a hit test depends on which `types` you specify and the order you specify them in. For details, see ARHitTestResult and the various ARHitTestResult.ResultType options.

