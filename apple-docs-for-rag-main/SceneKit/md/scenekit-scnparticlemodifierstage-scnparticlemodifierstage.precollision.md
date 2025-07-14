

- SceneKit
- SCNParticleModifierStage
-  SCNParticleModifierStage.preCollision 

Case

# SCNParticleModifierStage.preCollision

The stage before SceneKit simulates the results of collisions between particles and scene geometry.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
case preCollision
```

## Discussion

Insert a modifier block at this stage to alter the inputs to collision resolution. For example, if you modify the bounce factors of particles during this stage, SceneKit uses the modified factors to compute the bounce velocity of each particle.

## See Also

### Constants

case preDynamics

The stage before SceneKit simulates the motion of particles.

case postDynamics

The stage after SceneKit simulates the motion of particles.

case postCollision

The stage after SceneKit simulates the results of collisions between particles and scene geometry.

