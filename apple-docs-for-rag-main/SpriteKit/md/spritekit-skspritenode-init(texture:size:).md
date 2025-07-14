

- SpriteKit
- SKSpriteNode
-  init(texture:size:) 

Initializer

# init(texture:size:)

Initializes a textured sprite using an existing texture object but with a specified size.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
convenience init(
    texture: SKTexture?,
    size: CGSize
)
```

**watchOS**

``` source
convenience init(
    texture: SKTexture?,
    size: CGSize
)
```

## Parameters 

`texture`  

A SpriteKit texture.

`size`  

The size of the sprite in points.

## Return Value

A newly initialized sprite object.

## Discussion

The sprite is initialized using the texture, but the texture’s dimensions are not used. Instead, the size passed into the constructor method is used.

## See Also

### Creating a Sprite from a Texture

convenience init(texture: SKTexture?)

Initializes a textured sprite using an existing texture object.

init(texture: SKTexture?, color: UIColor, size: CGSize)

Initializes a textured sprite in color using an existing texture object.

convenience init(texture: SKTexture?, normalMap: SKTexture?)

Initializes a textured sprite with a normal map to simulate 3D lighting.

var texture: SKTexture?

The texture used to draw the sprite.

