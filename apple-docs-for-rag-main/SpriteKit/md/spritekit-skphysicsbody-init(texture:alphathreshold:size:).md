

- SpriteKit
- SKPhysicsBody
-  init(texture:alphaThreshold:size:) 

Initializer

# init(texture:alphaThreshold:size:)

Creates a physics body from the contents of a texture, capturing only the texels that exceed a specified transparency value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
init(
    texture: SKTexture,
    alphaThreshold: Float,
    size: CGSize
)
```

## Parameters 

`texture`  

The texture to analyze.

`alphaThreshold`  

The minimum alpha value for texels that should be part of the new physics body.

`size`  

The size of the physics body to return.

## Return Value

A new volume-based physics body.

## Discussion

Use this method when your sprite has a shape that you want replicated in its physics body. The texture is scaled to the new size and then analyzed. A new physics body is created that includes all of the texels in the texture whose alpha values equal or exceed the `alphaThreshold` parameter. The shape of this body attempts to strike a good balance between performance and accuracy. For example, fine details may be ignored if keeping them would cause a significant performance penalty.

## See Also

### Creating a Body from a Texture

Shaping a Physics Body to Match a Node’s Graphics

Shape a physics body to your graphics for the right blend of collision accuracy and performance.

init(texture: SKTexture, size: CGSize)

Creates a physics body from the contents of a texture.

