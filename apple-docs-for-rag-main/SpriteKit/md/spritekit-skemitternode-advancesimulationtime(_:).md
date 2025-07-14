

- SpriteKit
- SKEmitterNode
-  advanceSimulationTime(\_:) 

Instance Method

# advanceSimulationTime(\_:)

Advances the emitter particle simulation.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
func advanceSimulationTime(_ sec: TimeInterval)
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func advanceSimulationTime(_ sec: TimeInterval)
```

## Parameters 

`sec`  

The number of seconds to simulate.

## Discussion

Once added to a scene, an emitter node automatically creates new particles in new animation frames. This method allows you to artificially advance a running emitter’s simulation, causing it to generate new particles and advance any existing particles. The most common use for this method is to prepopulate an emitter node with particles after it is first added to a scene.

If an emitter is paused, either directly or by one of its parent nodes being paused, advanceSimulationTime(_:) has no effect. Listing 1 shows how to advance an emitter object while it is paused, by temporarily toggling its isPaused property while advancing the simulation.

Listing 1. Temporarily unpausing an emitter to advance simulation time

```
let emitter = SKEmitterNode()
let emitterPaused = emitter.isPaused
if emitterPaused {
    emitter.isPaused = false
}
emitter.advanceSimulationTime(5)
if emitterPaused {
    emitter.isPaused = true
}
```

Note that the isPaused property is inherited from a node’s parents, so even if the emitter hasn’t been explicitly paused but, for example, the scene has, this code will still work.

## See Also

### Controlling When Particles Are Created

func resetSimulation()

Removes all existing particles and restarts the simulation.

var particleBirthRate: CGFloat

The rate at which new particles are created.

var numParticlesToEmit: Int

The number of particles the emitter should emit before stopping.

