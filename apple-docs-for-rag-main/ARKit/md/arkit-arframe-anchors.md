

- ARKit
- ARFrame
-  anchors 

Instance Property

# anchors

The list of anchors representing positions tracked or objects detected in the scene.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
var anchors: [ARAnchor] { get }
```

## Discussion

You can manually add or remove anchors to track locations in the scene using the ARSession class. Depending on session configuration, ARKit may also add anchors, such as the origin of the world coordinate system or automatically detected planes.

## See Also

### Tracking and interacting with the real world

func raycastQuery(from: CGPoint, allowing: ARRaycastQuery.Target, alignment: ARRaycastQuery.TargetAlignment) -> ARRaycastQuery

Get a ray-cast query for a screen point.

func hitTest(CGPoint, types: ARHitTestResult.ResultType) -> [ARHitTestResult]

Searches for real-world objects or AR anchors in the captured camera image.

Deprecated

