

- SceneKit
- SCNParticlePropertyController
-  inputMode 

Instance Property

# inputMode

The mode that determines input values for the property controller’s animation.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var inputMode: SCNParticleInputMode { get set }
```

## Discussion

With the default input mode of SCNParticleInputMode.overLife, the animation timing for each particle is based on the particle’s life span. For example, consider an animation that reduces each particle’s opacity from `1.0` to `0.0`. By default, a particle begins with full opacity, and reduces its opacity completely by the end of its life span (regardless of the particle’s position and other properties). Change the input mode to make each particle’s opacity a function of a different measurement, such as distance from a specified point or one of the particle’s other properties. For more details, see SCNParticleInputMode.

## See Also

### Managing the Controller’s Animation

var animation: CAAnimation

The Core Animation object defining the behavior of the property animation.

var inputBias: CGFloat

An offset to add to the input value of the controller’s animation.

var inputScale: CGFloat

A factor for multiplying the input value of the controller’s animation.

var inputOrigin: SCNNode?

A node whose distance to each particle provides input values for the controller’s animation.

var inputProperty: SCNParticleSystem.ParticleProperty?

A particle property that provides input values for this property controller’s animation.

