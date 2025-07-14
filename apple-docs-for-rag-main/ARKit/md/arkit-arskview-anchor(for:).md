

- ARKit
- ARSKView
-  anchor(for:) 

Instance Method

# anchor(for:)

Returns the AR anchor associated with the specified SpriteKit node, if any.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
@MainActor
func anchor(for node: SKNode) -> ARAnchor?
```

## Parameters 

`node`  

A SpriteKit node in the view’s scene.

## Return Value

The ARAnchor object tracking the node, or `nil` if the node is not associated with an anchor or not in the view’s scene.

## See Also

### Mapping Content to Real-World Positions

func node(for: ARAnchor) -> SKNode?

Returns the SpriteKit node associated with the specified AR anchor, if any.

