

- SceneKit
- SCNParticlePropertyController
-  init(animation:) 

Initializer

# init(animation:)

Creates a particle property controller with the specified Core Animation animation.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOS

``` source
convenience init(animation: CAAnimation)
```

## Parameters 

`animation`  

A Core Animation object specifying the behavior of the property animation. Must not be nil.

You can use different CAAnimation subclasses to animate effects in different ways. For example, a CABasicAnimation instance transitions a property from one value to another, and a CAKeyframeAnimation instance transitions a property through a series of values. You use properties of the animation object to define its timing curve, repeat mode, and other options.

SceneKit ignores the keyPath, duration, and repeatCount properties of this animation object.

## Return Value

A new particle property controller.

## Discussion

To set up a particle property animation:

1.  Create a CAAnimation object defining how a property of each particle in the system changes over time.

2.  Create a particle property controller using the init(animation:) method.

3.  Attach the property controller to a particle system using the propertyControllers dictionary, choosing a key listed in Particle Property Keys to identify the particle property it animates.

For example, the following code sets up a controller to animate particle sizes:

```
// 1. Create and configure an animation object.
CAKeyframeAnimation *animation = [CAKeyframeAnimation animation];
animation.values = @[ @0.1, @1.0, @3.0, @0.5 ];

// 2. Create a property controller from the animation object.
SCNParticlePropertyController *controller =
    [SCNParticlePropertyController controllerWithAnimation:animation];

// 3. Assign the controller to a particle system, associating it with a particle property.
particleSystem.propertyControllers = @{ SCNParticlePropertySize: controller };
```

