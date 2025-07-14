

- ARKit
- ARSCNViewDelegate
-  renderer(\_:didAdd:for:) 

Instance Method

# renderer(\_:didAdd:for:)

Tells the delegate that a SceneKit node corresponding to a new AR anchor has been added to the scene.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
optional func renderer(
    _ renderer: any SCNSceneRenderer,
    didAdd node: SCNNode,
    for anchor: ARAnchor
)
```

## Parameters 

`renderer`  

The ARSCNView object rendering the scene.

`node`  

The newly added SceneKit node.

`anchor`  

The AR anchor corresponding to the node.

## Discussion

Depending on the session configuration, ARKit may automatically add anchors to a session. The view calls this method once for each new anchor. ARKit also calls this method to provide visual content for any ARAnchor objects you manually add using the session’s add(anchor:) method.

You can provide visual content for the anchor by attaching geometry (or other SceneKit features) to this node or by adding child nodes.

Alternatively, you can implement the renderer(_:nodeFor:) method to create your own node (or instance of an SCNNode subclass) for an anchor.

## See Also

### Handling Content Updates

func renderer(any SCNSceneRenderer, nodeFor: ARAnchor) -> SCNNode?

Asks the delegate to provide a SceneKit node corresponding to a newly added anchor.

func renderer(any SCNSceneRenderer, willUpdate: SCNNode, for: ARAnchor)

Tells the delegate that a SceneKit node’s properties will be updated to match the current state of its corresponding anchor.

func renderer(any SCNSceneRenderer, didUpdate: SCNNode, for: ARAnchor)

Tells the delegate that a SceneKit node’s properties have been updated to match the current state of its corresponding anchor.

func renderer(any SCNSceneRenderer, didRemove: SCNNode, for: ARAnchor)

Tells the delegate that the SceneKit node corresponding to a removed AR anchor has been removed from the scene.

