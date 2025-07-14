

- SpriteKit
- SKSpriteNode
-  init(imageNamed:normalMapped:) 

Initializer

# init(imageNamed:normalMapped:)

Initializes a textured sprite using an image file, optionally adding a normal map to simulate 3D lighting.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
convenience init(
    imageNamed name: String,
    normalMapped generateNormalMap: Bool
)
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
convenience init(
    imageNamed name: String,
    normalMapped generateNormalMap: Bool
)
```

## Parameters 

`name`  

The name of an image file stored in the app bundle.

`generateNormalMap`  

If true, a normal map is generated from the image texture without applying any filter to it (SKTextureNormalMapFilteringTypeNone). If false, no normal map is generated (matching the behavior of the spriteNodeWithImageNamed: class method).

## Return Value

A newly initialized sprite object.

## Discussion

The normal map is used only when lighting is enabled in the scene. For more information, see SKSpriteNode and SKLightNode.

## See Also

### Creating a Sprite from an Image Filename

Getting Started with Sprite Nodes

Learn the basics about using images, also known as sprites, with SpriteKit.

convenience init(imageNamed: String)

Initializes a textured sprite using an image file.

