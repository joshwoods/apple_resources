

- SceneKit
- SCNParticlePropertyController
-  animation 

Instance Property

# animation

The Core Animation object defining the behavior of the property animation.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOS

``` source
var animation: CAAnimation { get set }
```

## Discussion

You can use different CAAnimation subclasses to animate effects in different ways. For example, a CABasicAnimation transitions a property from one value to another, and a CAKeyframeAnimation transitions a property through a series of values. You use properties of the animation object to define its timing curve, repeat mode, and other options.

SceneKit ignores the keyPath property of this animation object. Instead, when you attach a property controller to a particle system’s propertyControllers dictionary, use one of the keys listed in Particle Property Keys to specify which particle property it animates. SceneKit also ignores the animation’s duration and repeatCount properties. Instead, the controller defines the behavior of the animation’s input value.

## See Also

### Managing the Controller’s Animation

var inputMode: SCNParticleInputMode

The mode that determines input values for the property controller’s animation.

var inputBias: CGFloat

An offset to add to the input value of the controller’s animation.

var inputScale: CGFloat

A factor for multiplying the input value of the controller’s animation.

var inputOrigin: SCNNode?

A node whose distance to each particle provides input values for the controller’s animation.

var inputProperty: SCNParticleSystem.ParticleProperty?

A particle property that provides input values for this property controller’s animation.

