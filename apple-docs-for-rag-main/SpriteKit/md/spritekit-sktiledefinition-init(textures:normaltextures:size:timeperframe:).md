

- SpriteKit
- SKTileDefinition
-  init(textures:normalTextures:size:timePerFrame:) 

Initializer

# init(textures:normalTextures:size:timePerFrame:)

Initializes a new tile definition with arrays of textures and normal textures for animation.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
init(
    textures: [SKTexture],
    normalTextures: [SKTexture],
    size: CGSize,
    timePerFrame: CGFloat
)
```

## Parameters 

`textures`  

An array of textures to reference for the definition’s content.

`normalTextures`  

An array of textures to reference for generating normals to simulate 3D lighting.

`size`  

The size of the tile in points.

`timePerFrame`  

The duration, in seconds, that each texture is displayed.

## Return Value

A new tile definition.

## See Also

### Creating an Animated Tile

init(textures: [SKTexture], size: CGSize, timePerFrame: CGFloat)

Initializes a new tile definition with an array of textures for animation.

