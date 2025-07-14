

- ARKit
- ARSCNViewDelegate
-  renderer(\_:didUpdate:for:) 

Instance Method

# renderer(\_:didUpdate:for:)

Tells the delegate that a SceneKit node’s properties have been updated to match the current state of its corresponding anchor.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
optional func renderer(
    _ renderer: any SCNSceneRenderer,
    didUpdate node: SCNNode,
    for anchor: ARAnchor
)
```

## Parameters 

`renderer`  

The ARSCNView object rendering the scene.

`node`  

The updated SceneKit node.

`anchor`  

The AR anchor corresponding to the node.

## Discussion

Depending on the session configuration, ARKit may automatically update anchors in a session. The view calls this method once for each updated anchor.

## See Also

### Handling Content Updates

func renderer(any SCNSceneRenderer, nodeFor: ARAnchor) -> SCNNode?

Asks the delegate to provide a SceneKit node corresponding to a newly added anchor.

func renderer(any SCNSceneRenderer, didAdd: SCNNode, for: ARAnchor)

Tells the delegate that a SceneKit node corresponding to a new AR anchor has been added to the scene.

func renderer(any SCNSceneRenderer, willUpdate: SCNNode, for: ARAnchor)

Tells the delegate that a SceneKit node’s properties will be updated to match the current state of its corresponding anchor.

func renderer(any SCNSceneRenderer, didRemove: SCNNode, for: ARAnchor)

Tells the delegate that the SceneKit node corresponding to a removed AR anchor has been removed from the scene.

