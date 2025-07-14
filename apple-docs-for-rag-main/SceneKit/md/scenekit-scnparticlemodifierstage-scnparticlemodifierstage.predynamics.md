

- SceneKit
- SCNParticleModifierStage
-  SCNParticleModifierStage.preDynamics 

Case

# SCNParticleModifierStage.preDynamics

The stage before SceneKit simulates the motion of particles.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
case preDynamics
```

## Discussion

Insert a modifier block at this stage to alter the inputs to the dynamics simulation. For example, if you modify the velocities of particles during this stage, SceneKit computes new positions for each particle based on its modified velocity.

## See Also

### Constants

case postDynamics

The stage after SceneKit simulates the motion of particles.

case preCollision

The stage before SceneKit simulates the results of collisions between particles and scene geometry.

case postCollision

The stage after SceneKit simulates the results of collisions between particles and scene geometry.

