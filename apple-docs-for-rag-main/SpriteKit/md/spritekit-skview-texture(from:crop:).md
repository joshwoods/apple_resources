

- SpriteKit
- SKView
-  texture(from:crop:) 

Instance Method

# texture(from:crop:)

Renders a portion of a node’s contents and returns the rendered image as a texture.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
@MainActor
func texture(
    from node: SKNode,
    crop: CGRect
) -> SKTexture?
```

## Parameters 

`node`  

The node object that is the root node of the tree you want to render to the texture.

`crop`  

A rectangle in the node’s coordinate system that describes the area to be rendered.

## Return Value

A SpriteKit texture that holds the rendered image.

## Mentioned in 

Creating a New Node By Rendering To a Texture

## Discussion

The node being rendered does not need to appear in the view’s presented scene. The new texture is created with a size equal to the size of the `crop` rectangle. If the node is not a scene node, it is rendered with a clear background color (``` [``SKColor ``` `clear]`).

## See Also

### Snapshotting Nodes to a Texture

func texture(from: SKNode) -> SKTexture?

Renders the contents of a node tree and returns the rendered image as a texture.

Creating a New Node By Rendering To a Texture

Render a portion of the node tree into a new texture.

