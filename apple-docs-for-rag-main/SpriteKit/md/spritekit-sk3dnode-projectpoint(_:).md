

- SpriteKit
- SK3DNode
-  projectPoint(\_:) 

Instance Method

# projectPoint(\_:)

Projects a point from the 3D world coordinate system of the SceneKit scene to the 2D viewport coordinate system of the SpriteKit node.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

**watchOS**

``` source
func projectPoint(_ point: vector_float3) -> vector_float3
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func projectPoint(_ point: vector_float3) -> vector_float3
```

## Parameters 

`point`  

A point in the world coordinate system of the Scene Kit scene.

## Return Value

The corresponding point in the SpriteKit node’s coordinate system.

## Discussion

The z-coordinate of the returned point describes the depth of the projected point relative to the near and far clipping planes of the viewing frustum (defined by the pointOfView property). Projecting a point on the near clipping plane returns a point whose z-coordinate is `0.0`; projecting a point on the far clipping plane returns a point whose z-coordinate is `1.0`.

The following Swift code illustrates how you might convert the position of a SceneKit node, `sphereNode`, in 3D space to the 2D coordinates of a SpriteKit SK3DNode, `node`. The code assumes that `sphereNode` is the first child node of the SceneKit scene’s rootNode.

```
if let sphereNode = node.scnScene?.rootNode.childNodes.first { 
    let location = node.projectPoint(vector_float3(Float(sphereNode.position.x),
                                                   Float(sphereNode.position.y),
                                                   Float(sphereNode.position.z)))
}
```

## See Also

### Projecting Points and Performing Hit-Testing

func hitTest(CGPoint, options: [String : Any]?) -> [SCNHitTestResult]

Searches the Scene Kit scene for objects corresponding to a point in the rendered image.

func unprojectPoint(vector_float3) -> vector_float3

Unprojects a point from the SpriteKit node’s 2D viewport coordinate system to the 3D world coordinate system of the SceneKit scene.

