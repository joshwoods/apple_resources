

- SceneKit
- SCNParticlePropertyController
-  inputOrigin 

Instance Property

# inputOrigin

A node whose distance to each particle provides input values for the controller’s animation.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
weak var inputOrigin: SCNNode? { get set }
```

## Discussion

This property applies only when the controller’s inputMode value is SCNParticleInputMode.overDistance. When you select that input mode, this property’s value must be a node in the scene containing the particle system; otherwise, SceneKit ignores this property. The default value is `nil`.

SceneKit calculates the distance between this node’s position vector (converted to the scene’s world coordinate space) and each particle and then uses the resulting value as the input to the controller’s animation. For example, if you use this option to animate particle opacity from `1.0` to `0.0`, all particles beyond a certain distance from the inputOrigin node are fully transparent—regardless of any random velocity or direction variations in reaching that distance.

To refine the relationship between a range of distances and a range of input values for the controller’s animation, use the inputBias and inputScale properties.

## See Also

### Managing the Controller’s Animation

var animation: CAAnimation

The Core Animation object defining the behavior of the property animation.

var inputMode: SCNParticleInputMode

The mode that determines input values for the property controller’s animation.

var inputBias: CGFloat

An offset to add to the input value of the controller’s animation.

var inputScale: CGFloat

A factor for multiplying the input value of the controller’s animation.

var inputProperty: SCNParticleSystem.ParticleProperty?

A particle property that provides input values for this property controller’s animation.

