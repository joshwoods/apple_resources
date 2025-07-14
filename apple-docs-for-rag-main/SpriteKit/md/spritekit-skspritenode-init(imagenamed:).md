

- SpriteKit
- SKSpriteNode
-  init(imageNamed:) 

Initializer

# init(imageNamed:)

Initializes a textured sprite using an image file.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
convenience init(imageNamed name: String)
```

**watchOS**

``` source
convenience init(imageNamed name: String)
```

## Parameters 

`name`  

The name of an image file stored in the app bundle.

## Return Value

A newly initialized sprite object.

## Mentioned in 

Resizing a Sprite in Nine Parts

## Discussion

This method creates a new texture object from the image file and assigns that texture to the texture property, the normalTexture properties is set to `nil`. The size property of the sprite is set to the dimensions of the image. The color property is set to white with an alpha of zero `(1.0,1.0,1.0,0.0)`.

## See Also

### Creating a Sprite from an Image Filename

Getting Started with Sprite Nodes

Learn the basics about using images, also known as sprites, with SpriteKit.

convenience init(imageNamed: String, normalMapped: Bool)

Initializes a textured sprite using an image file, optionally adding a normal map to simulate 3D lighting.

