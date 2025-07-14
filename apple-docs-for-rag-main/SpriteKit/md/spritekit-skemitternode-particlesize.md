

- SpriteKit
- SKEmitterNode
-  particleSize 

Instance Property

# particleSize

The starting size of each particle.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
var particleSize: CGSize { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var particleSize: CGSize { get set }
```

## Discussion

The default value is CGSizeZero. If set to the default, the size of the texture stored in the particleTexture property is used to determine the size of a particle. If a texture has not been assigned, you must set this property to a non-empty size.

## See Also

### Changing a Particle’s Source Image and Size

var particleTexture: SKTexture?

The texture to use to render a particle.

