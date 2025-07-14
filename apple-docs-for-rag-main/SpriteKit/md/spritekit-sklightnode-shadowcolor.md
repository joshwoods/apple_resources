

- SpriteKit
- SKLightNode
-  shadowColor 

Instance Property

# shadowColor

The color of any shadow cast by a sprite.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**macOS**

``` source
@MainActor
var shadowColor: NSColor { get set }
```

**watchOS**

``` source
var shadowColor: UIColor { get set }
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
var shadowColor: UIColor { get set }
```

## Discussion

The default color is black with an opacity (alpha) of `0.5`.

When lighting is calculated, shadows are created as if a ray was cast out from the light node’s position. If a sprite casts a shadow, the rays are blocked when they intersect with the sprite’s physics body. Otherwise, the sprite’s texture is used to generate a mask, and any pixel in the sprite node’s texture that has an alpha value that is nonzero blocks the light.

Shadows may be cast on content that is rendered prior to the sprite, even if that content does not otherwise interact with the light.

## See Also

### Configuring the Lighting Properties

var ambientColor: UIColor

The ambient color of the light.

var lightColor: UIColor

The diffuse and specular color of the light source.

var falloff: CGFloat

The exponent for the rate of decay of the light source.

