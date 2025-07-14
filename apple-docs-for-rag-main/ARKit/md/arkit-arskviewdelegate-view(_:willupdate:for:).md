

- ARKit
- ARSKViewDelegate
-  view(\_:willUpdate:for:) 

Instance Method

# view(\_:willUpdate:for:)

Tells the delegate that a SpriteKit node’s properties will be updated to match the current state of its corresponding anchor.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
optional func view(
    _ view: ARSKView,
    willUpdate node: SKNode,
    for anchor: ARAnchor
)
```

## Parameters 

`view`  

The ARSKView object rendering the scene.

`node`  

The updated SpriteKit node.

`anchor`  

The AR anchor corresponding to the node.

## Discussion

Depending on the session configuration, ARKit may automatically update anchors in a session. The view calls this method once for each updated anchor.

## See Also

### Handling Content Updates

func view(ARSKView, nodeFor: ARAnchor) -> SKNode?

Asks the delegate to provide a SpriteKit node corresponding to a newly added anchor.

func view(ARSKView, didAdd: SKNode, for: ARAnchor)

Tells the delegate that a SpriteKit node corresponding to a new AR anchor has been added to the scene.

func view(ARSKView, didUpdate: SKNode, for: ARAnchor)

Tells the delegate that a SpriteKit node’s properties have been updated to match the current state of its corresponding anchor.

func view(ARSKView, didRemove: SKNode, for: ARAnchor)

Tells the delegate that the SpriteKit node corresponding to an AR anchor has been removed from the scene.

