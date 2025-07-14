

- SpriteKit
- SKEmitterNode
-  particleTexture 

Instance Property

# particleTexture

The texture to use to render a particle.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var particleTexture: SKTexture? { get set }
```

**watchOS**

``` source
var particleTexture: SKTexture? { get set }
```

## Discussion

A particle is rendered as if it were a SKSpriteNode object. The default value is `nil`, which means a single-color rectangle is used to draw the particle. If a non-`nil` value is specified, then the texture is colorized and used to draw particles.

## See Also

### Changing a Particle’s Source Image and Size

var particleSize: CGSize

The starting size of each particle.

