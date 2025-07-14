

- SceneKit
-  SCNParticleEvent 

Enumeration

# SCNParticleEvent

Significant events in the life spans of simulate particles, used by the handle(_:forProperties:handler:) method.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
enum SCNParticleEvent
```

## Topics

### Constants

case birth

Occurs when new particles spawn.

case death

Occurs when particles reach the end of their life span.

case collision

Occurs when particles collide with scene geometry.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Modifying Particles in Response to Particle System Events

func handle(SCNParticleEvent, forProperties: [SCNParticleSystem.ParticleProperty], handler: SCNParticleEventBlock)

Adds a block that modifies particle properties, to be executed at a specified event in the lifetimes of particles in the system.

typealias SCNParticleEventBlock

The signature for blocks called by SceneKit in response to significant events during particle simulation, used by the handle(_:forProperties:handler:) method.

