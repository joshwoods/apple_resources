

- SpriteKit
- SKView
-  texture(from:) 

Instance Method

# texture(from:)

Renders the contents of a node tree and returns the rendered image as a texture.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
@MainActor
func texture(from node: SKNode) -> SKTexture?
```

## Parameters 

`node`  

The node object that is the root node of the tree you want to render to the texture.

## Return Value

A SpriteKit texture that holds the rendered image.

## Mentioned in 

Creating a New Node By Rendering To a Texture

Loading and Using Textures

## Discussion

The node being rendered does not need to appear in the view’s presented scene. The new texture is created with a size equal to the rectangle returned by the node’s calculateAccumulatedFrame() method. If the node is not a scene node, it is rendered with a clear background color (``` [``SKColor ``` `clear]`).

## See Also

### Snapshotting Nodes to a Texture

func texture(from: SKNode, crop: CGRect) -> SKTexture?

Renders a portion of a node’s contents and returns the rendered image as a texture.

Creating a New Node By Rendering To a Texture

Render a portion of the node tree into a new texture.

