

- SceneKit
- SCNParticleModifierStage
-  SCNParticleModifierStage.postCollision 

Case

# SCNParticleModifierStage.postCollision

The stage after SceneKit simulates the results of collisions between particles and scene geometry.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
case postCollision
```

## Discussion

Insert a modifier block at this stage to alter the output of collision resolution. For example, if you modify the velocities of particles during this stage, the modified velocities override the bounce velocity determined by SceneKit’s simulation.

## See Also

### Constants

case preDynamics

The stage before SceneKit simulates the motion of particles.

case postDynamics

The stage after SceneKit simulates the motion of particles.

case preCollision

The stage before SceneKit simulates the results of collisions between particles and scene geometry.

