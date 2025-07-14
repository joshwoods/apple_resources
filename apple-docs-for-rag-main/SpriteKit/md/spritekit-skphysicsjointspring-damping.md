

- SpriteKit
- SKPhysicsJointSpring
-  damping 

Instance Property

# damping

Defines how the spring’s motion should be damped due to the forces of friction.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var damping: CGFloat { get set }
```

## Discussion

The default value is `0.0`. Increasing the value increases the energy loss with each oscillation: there will be fewer and smaller oscillations and time taken for the spring to settle will decrease.

## See Also

### Configuring a Spring Joint

var frequency: CGFloat

Defines the frequency or stiffness characteristics of the spring.

