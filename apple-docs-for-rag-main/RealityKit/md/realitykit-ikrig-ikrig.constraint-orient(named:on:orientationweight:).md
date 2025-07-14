

- RealityKit
- IKRig
- IKRig.Constraint
-  orient(named:on:orientationWeight:) 

Type Method

# orient(named:on:orientationWeight:)

Creates a constraint with only an orientation demand.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
static func orient(
    named name: String,
    on jointName: String,
    orientationWeight: SIMD3 = [1, 1, 1]
) -> IKRig.Constraint
```

## Parameters 

`name`  

The rig unique name of the constraint

`jointName`  

The name of the joint to constrain.

`orientationWeight`  

The weight of the orientation demand.

