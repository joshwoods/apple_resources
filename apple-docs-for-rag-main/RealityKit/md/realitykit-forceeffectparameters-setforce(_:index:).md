

- RealityKit
- ForceEffectParameters
-  setForce(\_:index:) 

Instance Method

# setForce(\_:index:)

Sets the force for each rigid body.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
func setForce(
    _ force: SIMD3,
    index: Int
)
```

## Parameters 

`force`  

The force value.

`index`  

The index to the rigid body. The index should be in the range \[0, physicsBodyCount\].

## Discussion

Inside the force effect update function, you are responsible to compute and output the force by calling this function for each rigid body. If you omit this function for a rigid body, that rigid body gets zero force from the effect.

