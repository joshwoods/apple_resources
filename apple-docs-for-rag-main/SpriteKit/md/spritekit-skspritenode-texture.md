

- SpriteKit
- SKSpriteNode
-  texture 

Instance Property

# texture

The texture used to draw the sprite.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var texture: SKTexture? { get set }
```

**watchOS**

``` source
var texture: SKTexture? { get set }
```

## Discussion

If the value is `nil`, the sprite is drawn as a single-color rectangle using its color property. Otherwise, the texture is used to draw the sprite. The related properties affect how the texture is applied.

SpriteKit automatically generates a texture for sprites when they are initialized with init(imageNamed:).

## See Also

### Creating a Sprite from a Texture

convenience init(texture: SKTexture?)

Initializes a textured sprite using an existing texture object.

init(texture: SKTexture?, color: UIColor, size: CGSize)

Initializes a textured sprite in color using an existing texture object.

convenience init(texture: SKTexture?, size: CGSize)

Initializes a textured sprite using an existing texture object but with a specified size.

convenience init(texture: SKTexture?, normalMap: SKTexture?)

Initializes a textured sprite with a normal map to simulate 3D lighting.

