

- SpriteKit
- SKEmitterNode
-  particleAction 

Instance Property

# particleAction

An action executed by new particles.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
@NSCopying
var particleAction: SKAction? { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@NSCopying @MainActor
var particleAction: SKAction? { get set }
```

## Discussion

Although you do not have direct access to the particles created by SpriteKit, you can specify an action that all particles execute. Whenever a new particle is created, the emitter tells the particle to run that action. You can use actions to create very sophisticated behaviors.

For the purpose of using actions on particles, you can treat the particle as if it were a normal node. This means you can perform other interesting tricks, such as animating the particle’s textures.

Tip

Adding complex actions to particles can severely impact the performance of the particle emitter. Also, because the particles do not exist as an explicit node that you can manipulate, you cannot remove the actions from existing particles.

## See Also

### Animating Particles

Animating Particle Properties Across Disparate Values

Supply keyframe sequences to do linear or nonlinear particle animations.

