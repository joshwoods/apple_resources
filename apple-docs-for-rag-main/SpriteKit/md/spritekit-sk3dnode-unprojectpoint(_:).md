

- SpriteKit
- SK3DNode
-  unprojectPoint(\_:) 

Instance Method

# unprojectPoint(\_:)

Unprojects a point from the SpriteKit node’s 2D viewport coordinate system to the 3D world coordinate system of the SceneKit scene.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

**watchOS**

``` source
func unprojectPoint(_ point: vector_float3) -> vector_float3
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func unprojectPoint(_ point: vector_float3) -> vector_float3
```

## Parameters 

`point`  

A point in the SpriteKit node’s coordinate system.

## Return Value

The corresponding point in the world coordinate system of the SceneKit scene.

## Discussion

The z-coordinate of the `point` parameter describes the depth at which to unproject the point relative to the near and far clipping planes of the viewing frustum (defined by the SK3DNode property). Unprojecting a point whose z-coordinate is `0.0` returns a point on the near clipping plane; unprojecting a point whose z-coordinate is `1.0` returns a point on the far clipping plane.

A point in the SpriteKit node’s 2D viewport coordinate space can refer to any point along a line segment in the 3D SceneKit coordinate space. To test for scene contents along this line—for example, to find the geometry corresponding to a touch event—use the SK3DNode method.

The following Swift code shows how you might convert the location of an iOS touch event inside an SK3DNode, `node`, to the 3D coordinates within its SceneKit scene. The resulting value, `sceneKitCoordinates`, is given a `z` of `0.5`, meaning that the coordinate is midway between the near and far clipping planes. You could use this value to set the position of an object within the SceneKit scene.

```
override func touchesMoved(_ touches: Set, with event: UIEvent?) {
    guard let touch = touches.first else {
        return
    }

    let location = touch.location(in: node)
    let scale = Float(UIScreen.main.scale)

    let sceneKitCoordinates = node.unprojectPoint(vector_float3(Float(location.x) * scale,
                                                                Float(location.y) * scale,
                                                                0.5))
}
```

## See Also

### Projecting Points and Performing Hit-Testing

func hitTest(CGPoint, options: [String : Any]?) -> [SCNHitTestResult]

Searches the Scene Kit scene for objects corresponding to a point in the rendered image.

func projectPoint(vector_float3) -> vector_float3

Projects a point from the 3D world coordinate system of the SceneKit scene to the 2D viewport coordinate system of the SpriteKit node.

