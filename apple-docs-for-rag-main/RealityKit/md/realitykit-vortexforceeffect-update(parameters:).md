

- RealityKit
- VortexForceEffect
-  update(parameters:) 

Instance Method

# update(parameters:)

Calculates the vortex forces for rigid bodies from the force effect.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
func update(parameters: inout ForceEffectParameters)
```

## Parameters 

`parameters`  

On input, the parameters that calculate forces to the affected physics bodies; on output, the updates to those forces.

## Discussion

The framework automatically calls this method for you at each physics simulation step, so you don’t need to call it yourself.

