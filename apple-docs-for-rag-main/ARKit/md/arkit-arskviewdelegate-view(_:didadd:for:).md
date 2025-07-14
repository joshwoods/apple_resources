

- ARKit
- ARSKViewDelegate
-  view(\_:didAdd:for:) 

Instance Method

# view(\_:didAdd:for:)

Tells the delegate that a SpriteKit node corresponding to a new AR anchor has been added to the scene.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
optional func view(
    _ view: ARSKView,
    didAdd node: SKNode,
    for anchor: ARAnchor
)
```

## Parameters 

`view`  

The ARSKView object rendering the scene.

`node`  

The newly added SpriteKit node.

`anchor`  

The AR anchor corresponding to the node.

## Discussion

Depending on the session configuration, ARKit may automatically add anchors to a session. The view calls this method once for each new anchor. ARKit also calls this method to provide visual content for any ARAnchor objects you manually add using the session’s add(anchor:) method.

You can provide visual content for the anchor by adding child nodes.

Alternatively, you can implement the view(_:nodeFor:) method to create your own node (or instance of an SKNode subclass) for an anchor.

## See Also

### Handling Content Updates

func view(ARSKView, nodeFor: ARAnchor) -> SKNode?

Asks the delegate to provide a SpriteKit node corresponding to a newly added anchor.

func view(ARSKView, willUpdate: SKNode, for: ARAnchor)

Tells the delegate that a SpriteKit node’s properties will be updated to match the current state of its corresponding anchor.

func view(ARSKView, didUpdate: SKNode, for: ARAnchor)

Tells the delegate that a SpriteKit node’s properties have been updated to match the current state of its corresponding anchor.

func view(ARSKView, didRemove: SKNode, for: ARAnchor)

Tells the delegate that the SpriteKit node corresponding to an AR anchor has been removed from the scene.

