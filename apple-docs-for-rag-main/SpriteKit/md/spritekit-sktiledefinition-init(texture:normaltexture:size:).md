

- SpriteKit
- SKTileDefinition
-  init(texture:normalTexture:size:) 

Initializer

# init(texture:normalTexture:size:)

Initializes a new tile definition with a single texture and separate normal texture for simulating 3D lighting.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
init(
    texture: SKTexture,
    normalTexture: SKTexture,
    size: CGSize
)
```

## Parameters 

`texture`  

The texture to reference for the definition’s content.

`normalTexture`  

The texture to reference for generating normals to simulate 3D lighting.

`size`  

The size of the tile in points.

## Return Value

A new tile definition.

