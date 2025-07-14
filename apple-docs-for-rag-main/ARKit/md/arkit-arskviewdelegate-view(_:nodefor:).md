

- ARKit
- ARSKViewDelegate
-  view(\_:nodeFor:) 

Instance Method

# view(\_:nodeFor:)

Asks the delegate to provide a SpriteKit node corresponding to a newly added anchor.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
optional func view(
    _ view: ARSKView,
    nodeFor anchor: ARAnchor
) -> SKNode?
```

## Parameters 

`view`  

The ARSKView object rendering the scene.

`anchor`  

The anchor for which a node is requested.

## Return Value

A new SpriteKit node, which ARKit will add to the scene and update to follow its corresponding AR anchor.

## Mentioned in 

Providing 2D Virtual Content with SpriteKit

## Discussion

Depending on the session configuration, ARKit may automatically add anchors to a session, such as the origin of the world coordinate system and detected planes. ARKit also calls this method to provide visual content for any ARAnchor objects you manually add using the session’s add(anchor:) method.

You can implement this method to provide a new SKNode object (or instance of any system or custom SKNode subclass) you plan to use as a visual representation of the anchor.

Note that ARKit controls the node’s position, rotation, and scale to simulate a billboarded 3D effect even for 2D sprites. If you provide a `SKTransformLayer` node, ARKit applies a 3D transformation.

Alternatively, if you do not implement this method, ARKit creates an empty node, and you can implement the view(_:didAdd:for:) method instead to provide visual content by adding children to that node.

## See Also

### Handling Content Updates

func view(ARSKView, didAdd: SKNode, for: ARAnchor)

Tells the delegate that a SpriteKit node corresponding to a new AR anchor has been added to the scene.

func view(ARSKView, willUpdate: SKNode, for: ARAnchor)

Tells the delegate that a SpriteKit node’s properties will be updated to match the current state of its corresponding anchor.

func view(ARSKView, didUpdate: SKNode, for: ARAnchor)

Tells the delegate that a SpriteKit node’s properties have been updated to match the current state of its corresponding anchor.

func view(ARSKView, didRemove: SKNode, for: ARAnchor)

Tells the delegate that the SpriteKit node corresponding to an AR anchor has been removed from the scene.

