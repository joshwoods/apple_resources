

- SceneKit
- SCNSceneRenderer
-  hitTest(\_:options:) 

Instance Method

# hitTest(\_:options:)

Searches the renderer’s scene for objects corresponding to a point in the rendered image.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func hitTest(
    _ point: CGPoint,
    options: [SCNHitTestOption : Any]? = nil
) -> [SCNHitTestResult]
```

**Required**

## Parameters 

`point`  

A point in the screen-space (view, layer, or GPU viewport) coordinate system of the scene renderer.

`options`  

A dictionary of options affecting the search. See Hit Testing Options Keys for acceptable values.

## Return Value

An array of SCNHitTestResult objects representing search results.

## Discussion

A 2D point in the rendered screen coordinate space can refer to any point along a line segment in the 3D scene coordinate space. Hit-testing is the process of finding elements of a scene located along this line segment. For example, you can use this method to find the geometry corresponding to a click event in a SceneKit view.

## See Also

### Working With Projected Scene Contents

struct SCNHitTestOption

Options affecting the behavior of SceneKit hit-testing methods.

func isNode(SCNNode, insideFrustumOf: SCNNode) -> Bool

Returns a Boolean value indicating whether a node might be visible from a specified point of view.

**Required**

func nodesInsideFrustum(of: SCNNode) -> [SCNNode]

Returns all nodes that might be visible from a specified point of view.

**Required**

func projectPoint(SCNVector3) -> SCNVector3

Projects a point from the 3D world coordinate system of the scene to the 2D pixel coordinate system of the renderer.

**Required**

func unprojectPoint(SCNVector3) -> SCNVector3

Unprojects a point from the 2D pixel coordinate system of the renderer to the 3D world coordinate system of the scene.

**Required**

