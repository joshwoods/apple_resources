

- SceneKit
- SCNParticleModifierStage
-  SCNParticleModifierStage.postDynamics 

Case

# SCNParticleModifierStage.postDynamics

The stage after SceneKit simulates the motion of particles.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
case postDynamics
```

## Discussion

Insert a modifier block at this stage to alter the output of the dynamics simulation. For example, if you modify the positions of particles during this stage, the modified positions override those determined by SceneKit’s simulation.

## See Also

### Constants

case preDynamics

The stage before SceneKit simulates the motion of particles.

case preCollision

The stage before SceneKit simulates the results of collisions between particles and scene geometry.

case postCollision

The stage after SceneKit simulates the results of collisions between particles and scene geometry.

