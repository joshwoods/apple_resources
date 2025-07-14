

- SpriteKit
- SK3DNode
-  hitTest(\_:options:) 

Instance Method

# hitTest(\_:options:)

Searches the Scene Kit scene for objects corresponding to a point in the rendered image.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

**watchOS**

``` source
func hitTest(
    _ point: CGPoint,
    options: [String : Any]? = nil
) -> [SCNHitTestResult]
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func hitTest(
    _ point: CGPoint,
    options: [String : Any]? = nil
) -> [SCNHitTestResult]
```

## Parameters 

`point`  

A point in the viewport coordinate system of the SpriteKit node.

`options`  

A dictionary of options affecting the search. See Hit Testing Options Keys for acceptable values.

## Return Value

An array of SCNHitTestResult objects representing search results.

## Discussion

A point in the SpriteKit node’s 2D viewport coordinate space can refer to any point along a line segment in the 3D SceneKit coordinate space. Hit-testing is the process of finding elements of a scene located along this line segment. For example, you can use this method to find the geometry corresponding to a touch event.

## See Also

### Projecting Points and Performing Hit-Testing

func projectPoint(vector_float3) -> vector_float3

Projects a point from the 3D world coordinate system of the SceneKit scene to the 2D viewport coordinate system of the SpriteKit node.

func unprojectPoint(vector_float3) -> vector_float3

Unprojects a point from the SpriteKit node’s 2D viewport coordinate system to the 3D world coordinate system of the SceneKit scene.

