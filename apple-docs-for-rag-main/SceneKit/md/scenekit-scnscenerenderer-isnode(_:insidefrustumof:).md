

- SceneKit
- SCNSceneRenderer
-  isNode(\_:insideFrustumOf:) 

Instance Method

# isNode(\_:insideFrustumOf:)

Returns a Boolean value indicating whether a node might be visible from a specified point of view.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
func isNode(
    _ node: SCNNode,
    insideFrustumOf pointOfView: SCNNode
) -> Bool
```

**Required**

## Parameters 

`node`  

The node whose visibility is to be tested.

`pointOfView`  

A node defining a point of view, as used by the pointOfView property.

## Return Value

true if the bounding box of the tested node intersects the view frustum defined by the `pointOfView` node; otherwise, false.

## Discussion

Any node containing a camera or spotlight may serve as a point of view (see the pointOfView property for details). Such a node defines a *viewing frustum*—a portion of the scene’s coordinate space, shaped like a truncated pyramid, that encloses all points visible from that point of view.

Use this method to test whether a node lies within the viewing frustum defined by another node (which may or may not be the scene renderer’s current pointOfView node). For example, in a game scene containing multiple camera nodes, you could use this method to determine which camera is currently best for viewing a moving player character.

Note that this method does not perform occlusion testing. That is, it returns true if the tested node lies within the specified viewing frustum regardless of whether that node’s contents are obscured by other geometry.

## See Also

### Working With Projected Scene Contents

func hitTest(CGPoint, options: [SCNHitTestOption : Any]?) -> [SCNHitTestResult]

Searches the renderer’s scene for objects corresponding to a point in the rendered image.

**Required**

struct SCNHitTestOption

Options affecting the behavior of SceneKit hit-testing methods.

func nodesInsideFrustum(of: SCNNode) -> [SCNNode]

Returns all nodes that might be visible from a specified point of view.

**Required**

func projectPoint(SCNVector3) -> SCNVector3

Projects a point from the 3D world coordinate system of the scene to the 2D pixel coordinate system of the renderer.

**Required**

func unprojectPoint(SCNVector3) -> SCNVector3

Unprojects a point from the 2D pixel coordinate system of the renderer to the 3D world coordinate system of the scene.

**Required**

