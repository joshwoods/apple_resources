

- SceneKit
- SCNSceneRenderer
-  unprojectPoint(\_:) 

Instance Method

# unprojectPoint(\_:)

Unprojects a point from the 2D pixel coordinate system of the renderer to the 3D world coordinate system of the scene.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
func unprojectPoint(_ point: SCNVector3) -> SCNVector3
```

**Required**

## Parameters 

`point`  

A point in the screen-space (view, layer, or GPU viewport) coordinate system of the scene renderer.

## Return Value

The corresponding point in the world coordinate system of the renderer’s scene.

## Discussion

The z-coordinate of the `point` parameter describes the depth at which to unproject the point relative to the near and far clipping planes of the renderer’s viewing frustum (defined by its pointOfView node). Unprojecting a point whose z-coordinate is `0.0` returns a point on the near clipping plane; unprojecting a point whose z-coordinate is `1.0` returns a point on the far clipping plane.

A 2D point in the rendered screen coordinate space can refer to any point along a line segment in the 3D scene coordinate space. To test for scene contents along this line—for example, to find the geometry corresponding to the location of a click event in a view—use the hitTest(_:options:) method.

## See Also

### Working With Projected Scene Contents

func hitTest(CGPoint, options: [SCNHitTestOption : Any]?) -> [SCNHitTestResult]

Searches the renderer’s scene for objects corresponding to a point in the rendered image.

**Required**

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

