

- SceneKit
- SCNParticleEvent
-  SCNParticleEvent.death 

Case

# SCNParticleEvent.death

Occurs when particles reach the end of their life span.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
case death
```

## Discussion

SceneKit calls your event handler block immediately before removing dead particles from the scene.

## See Also

### Constants

case birth

Occurs when new particles spawn.

case collision

Occurs when particles collide with scene geometry.

