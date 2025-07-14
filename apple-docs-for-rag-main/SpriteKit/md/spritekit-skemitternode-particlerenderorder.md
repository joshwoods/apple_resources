

- SpriteKit
- SKEmitterNode
-  particleRenderOrder 

Instance Property

# particleRenderOrder

The order in which the emitter’s particles are rendered.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

**watchOS**

``` source
var particleRenderOrder: SKParticleRenderOrder { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var particleRenderOrder: SKParticleRenderOrder { get set }
```

## Discussion

The default value is SKParticleRenderOrder.oldestLast.

## See Also

### Controlling the Rendering Order of an Emitter’s Particles

enum SKParticleRenderOrder

The order to use when the emitter’s particles are rendered.

