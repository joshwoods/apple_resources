

- SpriteKit
- SKPhysicsJointSpring
-  frequency 

Instance Property

# frequency

Defines the frequency or stiffness characteristics of the spring.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var frequency: CGFloat { get set }
```

## Discussion

The default value is `0.0`, creating a rigid joint between the spring’s two bodies. Setting the frequency to a low value, for example `0.5`, creates a spring with slow oscillations that will settle slowly. Setting the frequency to a high value, for example `10.0`, creates a stiffer spring with faster and fewer oscillations.

## See Also

### Configuring a Spring Joint

var damping: CGFloat

Defines how the spring’s motion should be damped due to the forces of friction.

