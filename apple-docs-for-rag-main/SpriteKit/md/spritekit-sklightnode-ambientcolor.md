

- SpriteKit
- SKLightNode
-  ambientColor 

Instance Property

# ambientColor

The ambient color of the light.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
var ambientColor: UIColor { get set }
```

**macOS**

``` source
@MainActor
var ambientColor: NSColor { get set }
```

**watchOS**

``` source
var ambientColor: UIColor { get set }
```

## Discussion

The alpha value of the color is ignored. The default color is black, meaning that the light does not have an ambient component. The ambient component of the light is not affected by the light’s falloff property, nor is it affected by any normal map (normalTexture) on the sprite node.

## See Also

### Configuring the Lighting Properties

var lightColor: UIColor

The diffuse and specular color of the light source.

var shadowColor: UIColor

The color of any shadow cast by a sprite.

var falloff: CGFloat

The exponent for the rate of decay of the light source.

