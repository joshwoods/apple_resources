

- SpriteKit
- SKEmitterNode
-  numParticlesToEmit 

Instance Property

# numParticlesToEmit

The number of particles the emitter should emit before stopping.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
var numParticlesToEmit: Int { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var numParticlesToEmit: Int { get set }
```

## Mentioned in 

Creating Particle Effects

## Discussion

The default value is `0`, which indicates that emitter creates an endless stream of particles. If a non-zero value is provided, then the emitter stops generating particles after it has created the specified number of particles.

## See Also

### Controlling When Particles Are Created

func advanceSimulationTime(TimeInterval)

Advances the emitter particle simulation.

func resetSimulation()

Removes all existing particles and restarts the simulation.

var particleBirthRate: CGFloat

The rate at which new particles are created.

