

- ARKit
- ARSCNViewDelegate
-  renderer(\_:nodeFor:) 

Instance Method

# renderer(\_:nodeFor:)

Asks the delegate to provide a SceneKit node corresponding to a newly added anchor.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
optional func renderer(
    _ renderer: any SCNSceneRenderer,
    nodeFor anchor: ARAnchor
) -> SCNNode?
```

## Parameters 

`renderer`  

The ARSCNView object rendering the scene.

`anchor`  

The anchor for which a node is requested.

## Return Value

A new SceneKit node, which ARKit will add to the scene and update to follow its corresponding AR anchor.

## Discussion

Depending on the session configuration, ARKit may automatically add anchors to a session. ARKit also calls this method to provide visual content for any ARAnchor objects you manually add using the session’s add(anchor:) method.

You can implement this method to provide a new SCNNode object (or instance of an SCNNode subclass) containing any attachments you plan to use as a visual representation of the anchor. Note that ARKit controls the node’s visibility and its transform property, so you may find it useful to add child nodes or adjust the node’s pivot property to maintain any changes to position or orientation that you make.

If you return `nil` from this method, no node is added to the scene.

Alternatively, if you do not implement this method, ARKit creates an empty node, and you can implement the renderer(_:didAdd:for:) method instead to provide visual content by attaching it to that node.

## See Also

### Handling Content Updates

func renderer(any SCNSceneRenderer, didAdd: SCNNode, for: ARAnchor)

Tells the delegate that a SceneKit node corresponding to a new AR anchor has been added to the scene.

func renderer(any SCNSceneRenderer, willUpdate: SCNNode, for: ARAnchor)

Tells the delegate that a SceneKit node’s properties will be updated to match the current state of its corresponding anchor.

func renderer(any SCNSceneRenderer, didUpdate: SCNNode, for: ARAnchor)

Tells the delegate that a SceneKit node’s properties have been updated to match the current state of its corresponding anchor.

func renderer(any SCNSceneRenderer, didRemove: SCNNode, for: ARAnchor)

Tells the delegate that the SceneKit node corresponding to a removed AR anchor has been removed from the scene.

