

- SceneKit
- SCNParticleEvent
-  SCNParticleEvent.collision 

Case

# SCNParticleEvent.collision

Occurs when particles collide with scene geometry.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
case collision
```

## Discussion

SceneKit calls your event handler block immediately after resolving the collision.

## See Also

### Constants

case birth

Occurs when new particles spawn.

case death

Occurs when particles reach the end of their life span.

