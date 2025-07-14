

- SpriteKit
- SKSpriteNode
-  init(texture:color:size:) 

Initializer

# init(texture:color:size:)

Initializes a textured sprite in color using an existing texture object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**macOS**

``` source
@MainActor
init(
    texture: SKTexture?,
    color: NSColor,
    size: CGSize
)
```

**watchOS**

``` source
init(
    texture: SKTexture?,
    color: UIColor,
    size: CGSize
)
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
init(
    texture: SKTexture?,
    color: UIColor,
    size: CGSize
)
```

## Parameters 

`texture`  

A texture to apply to the sprite.

`color`  

The color for the new sprite.

`size`  

The size for the new sprite.

## Return Value

A newly initialized sprite object.

## Discussion

To colorize your texture, you also need to set the colorBlendFactor property of the sprite.

## See Also

### Creating a Sprite from a Texture

convenience init(texture: SKTexture?)

Initializes a textured sprite using an existing texture object.

convenience init(texture: SKTexture?, size: CGSize)

Initializes a textured sprite using an existing texture object but with a specified size.

convenience init(texture: SKTexture?, normalMap: SKTexture?)

Initializes a textured sprite with a normal map to simulate 3D lighting.

var texture: SKTexture?

The texture used to draw the sprite.

