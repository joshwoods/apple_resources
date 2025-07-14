

- SpriteKit
- SKSpriteNode
-  init(texture:normalMap:) 

Initializer

# init(texture:normalMap:)

Initializes a textured sprite with a normal map to simulate 3D lighting.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
convenience init(
    texture: SKTexture?,
    normalMap: SKTexture?
)
```

**watchOS**

``` source
convenience init(
    texture: SKTexture?,
    normalMap: SKTexture?
)
```

## Parameters 

`texture`  

A SpriteKit texture used to draw the sprite.

`normalMap`  

A SpriteKit texture used to add lighting behavior to the sprite.

## Return Value

A newly initialized sprite object.

## See Also

### Creating a Sprite from a Texture

convenience init(texture: SKTexture?)

Initializes a textured sprite using an existing texture object.

init(texture: SKTexture?, color: UIColor, size: CGSize)

Initializes a textured sprite in color using an existing texture object.

convenience init(texture: SKTexture?, size: CGSize)

Initializes a textured sprite using an existing texture object but with a specified size.

var texture: SKTexture?

The texture used to draw the sprite.

