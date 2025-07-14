

- SpriteKit
- SKLightNode
-  lightColor 

Instance Property

# lightColor

The diffuse and specular color of the light source.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**macOS**

``` source
@MainActor
var lightColor: NSColor { get set }
```

**watchOS**

``` source
var lightColor: UIColor { get set }
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
var lightColor: UIColor { get set }
```

## Discussion

The default value is white.

If you are using custom shaders, you can substitute an SKUniform object instead.

## See Also

### Configuring the Lighting Properties

var ambientColor: UIColor

The ambient color of the light.

var shadowColor: UIColor

The color of any shadow cast by a sprite.

var falloff: CGFloat

The exponent for the rate of decay of the light source.

