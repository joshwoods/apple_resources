

- SceneKit
- SCNSceneRenderer
-  projectPoint(\_:) 

Instance Method

# projectPoint(\_:)

Projects a point from the 3D world coordinate system of the scene to the 2D pixel coordinate system of the renderer.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
func projectPoint(_ point: SCNVector3) -> SCNVector3
```

**Required**

## Parameters 

`point`  

A point in the world coordinate system of the renderer’s scene.

## Return Value

The corresponding point in the screen-space (view, layer, or GPU viewport) coordinate system of the scene renderer.

## Discussion

The z-coordinate of the returned point describes the depth of the projected point relative to the near and far clipping planes of the renderer’s viewing frustum (defined by its pointOfView node). Projecting a point on the near clipping plane returns a point whose z-coordinate is `0.0`; projecting a point on the far clipping plane returns a point whose z-coordinate is `1.0`.

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

func unprojectPoint(SCNVector3) -> SCNVector3

Unprojects a point from the 2D pixel coordinate system of the renderer to the 3D world coordinate system of the scene.

**Required**

