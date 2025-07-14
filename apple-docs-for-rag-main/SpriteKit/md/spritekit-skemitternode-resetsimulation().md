

- SpriteKit
- SKEmitterNode
-  resetSimulation() 

Instance Method

# resetSimulation()

Removes all existing particles and restarts the simulation.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
func resetSimulation()
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func resetSimulation()
```

## Discussion

Resetting the simulation clears the internal state of the simulation.

## See Also

### Controlling When Particles Are Created

func advanceSimulationTime(TimeInterval)

Advances the emitter particle simulation.

var particleBirthRate: CGFloat

The rate at which new particles are created.

var numParticlesToEmit: Int

The number of particles the emitter should emit before stopping.

