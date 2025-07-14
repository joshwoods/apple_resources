

- RealityKit
- IKRig
- IKRig.Constraint
-  parent(named:on:positionWeight:orientationWeight:) 

Type Method

# parent(named:on:positionWeight:orientationWeight:)

Creates a constraint with both a positional and an orientational demands.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
static func parent(
    named name: String,
    on jointName: String,
    positionWeight: SIMD3 = [1, 1, 1],
    orientationWeight: SIMD3 = [1, 1, 1]
) -> IKRig.Constraint
```

## Parameters 

`name`  

The rig unique name of the constraint

`jointName`  

The name of the joint to constrain.

`positionWeight`  

The weight of the position demand.

`orientationWeight`  

The weight of the orientation demand.

