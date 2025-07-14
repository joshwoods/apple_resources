

- RealityKit
- IKRig
- IKRig.Constraint
-  point(named:on:positionWeight:) 

Type Method

# point(named:on:positionWeight:)

Creates a constraint with only a positional demand.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
static func point(
    named name: String,
    on jointName: String,
    positionWeight: SIMD3 = [1, 1, 1]
) -> IKRig.Constraint
```

## Parameters 

`name`  

The rig unique name of the constraint

`jointName`  

The name of the joint to constrain.

`positionWeight`  

The weight of the position demand.

