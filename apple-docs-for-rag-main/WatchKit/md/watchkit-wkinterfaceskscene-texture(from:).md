

- WatchKit
- WKInterfaceSKScene
-  texture(from:) 

Instance Method

# texture(from:)

Renders the contents of a node tree and returns the rendered image as a SpriteKit texture.

watchOS 3.0+

``` source
func texture(from node: SKNode) -> SKTexture?
```

## Parameters 

`node`  

A node object representing the root node of the tree to be render to the texture.

## Return Value

A SpriteKit texture that holds the rendered image.

## Discussion

The `node` being rendered does not need to appear in the interface’s presented scene. The new texture is created with a size equal to the rectangle returned by the `node`’s calculateAccumulatedFrame() method. If the `node` is not a scene node, it is rendered with a clear background color (`[SKColor clearColor]`).

## See Also

### Snapshotting Nodes to a Texture

func texture(from: SKNode, crop: CGRect) -> SKTexture?

Renders a portion of a node’s contents and returns the rendered image as a SpriteKit texture.

