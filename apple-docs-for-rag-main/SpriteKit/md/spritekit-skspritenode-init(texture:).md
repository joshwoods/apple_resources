

- SpriteKit
- SKSpriteNode
-  init(texture:) 

Initializer

# init(texture:)

Initializes a textured sprite using an existing texture object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
convenience init(texture: SKTexture?)
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
convenience init(texture: SKTexture?)
```

## Parameters 

`texture`  

A SpriteKit texture.

## Return Value

A newly initialized sprite object.

## Discussion

The size property of the sprite is set to the dimensions of the texture. The color property is set to white with an alpha of zero `(1.0,1.0,1.0,0.0)`.

## See Also

### Creating a Sprite from a Texture

init(texture: SKTexture?, color: UIColor, size: CGSize)

Initializes a textured sprite in color using an existing texture object.

convenience init(texture: SKTexture?, size: CGSize)

Initializes a textured sprite using an existing texture object but with a specified size.

convenience init(texture: SKTexture?, normalMap: SKTexture?)

Initializes a textured sprite with a normal map to simulate 3D lighting.

var texture: SKTexture?

The texture used to draw the sprite.

