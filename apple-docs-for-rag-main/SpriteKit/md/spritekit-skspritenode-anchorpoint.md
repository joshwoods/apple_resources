

- SpriteKit
- SKSpriteNode
-  anchorPoint 

Instance Property

# anchorPoint

Defines the point in the sprite that corresponds to the node’s position.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var anchorPoint: CGPoint { get set }
```

**watchOS**

``` source
var anchorPoint: CGPoint { get set }
```

## Mentioned in 

Animating a Sprite by Changing its Texture

Using the Anchor Point to Move a Sprite

## Discussion

You specify the value for this property in the unit coordinate space. The default value is `(0.5,0.5)`, which means that the sprite is centered on its position.

## See Also

### Setting a Sprite’s Size and Position

Using the Anchor Point to Move a Sprite

Learn how the anchor point affects a sprite’s position.

var size: CGSize

The dimensions of the sprite, in points.

func scale(to: CGSize)

Scales the sprite node to a specified size.

