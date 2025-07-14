

- SceneKit
- SCNParticlePropertyController
-  inputBias 

Instance Property

# inputBias

An offset to add to the input value of the controller’s animation.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var inputBias: CGFloat { get set }
```

## Discussion

Use this property and the inputScale property to pre-process input values to the controller’s animation. For example, if you use the SCNParticleInputMode.overDistance option to animate a particle’s opacity as a function of its distance from a specified point, a bias specifies the minimum distance at which the animation’s fromValue property or first keyframe value takes effect.

The default value is `0.0`, leaving the input value to the animation unchanged. The range of possible values depends on the controller’s animation.

## See Also

### Managing the Controller’s Animation

var animation: CAAnimation

The Core Animation object defining the behavior of the property animation.

var inputMode: SCNParticleInputMode

The mode that determines input values for the property controller’s animation.

var inputScale: CGFloat

A factor for multiplying the input value of the controller’s animation.

var inputOrigin: SCNNode?

A node whose distance to each particle provides input values for the controller’s animation.

var inputProperty: SCNParticleSystem.ParticleProperty?

A particle property that provides input values for this property controller’s animation.

