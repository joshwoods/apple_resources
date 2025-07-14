

- SpriteKit
- SKLightNode
-  falloff 

Instance Property

# falloff

The exponent for the rate of decay of the light source.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**watchOS**

``` source
var falloff: CGFloat { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var falloff: CGFloat { get set }
```

## Discussion

The default value is `1.0`, which means the light decays linearly with distance. The value must be a positive number less than or equal to `1.0`.

## See Also

### Configuring the Lighting Properties

var ambientColor: UIColor

The ambient color of the light.

var lightColor: UIColor

The diffuse and specular color of the light source.

var shadowColor: UIColor

The color of any shadow cast by a sprite.

