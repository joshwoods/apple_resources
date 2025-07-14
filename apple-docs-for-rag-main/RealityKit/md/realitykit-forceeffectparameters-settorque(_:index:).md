

- RealityKit
- ForceEffectParameters
-  setTorque(\_:index:) 

Instance Method

# setTorque(\_:index:)

Sets the torque for each rigid body.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
func setTorque(
    _ torque: SIMD3,
    index: Int
)
```

## Parameters 

`torque`  

The torque value.

`index`  

The index to the rigid body. The index should be in the range \[0, physicsBodyCount\].

## Discussion

Inside the force effect update function, you are responsible to compute and output the torque by calling this function for each rigid body. If you omit this function for a rigid body, that rigid body gets zero torque from the effect.

