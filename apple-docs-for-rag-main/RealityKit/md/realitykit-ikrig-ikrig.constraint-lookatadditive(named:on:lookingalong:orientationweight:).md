

- RealityKit
- IKRig
- IKRig.Constraint
-  lookAtAdditive(named:on:lookingAlong:orientationWeight:) 

Type Method

# lookAtAdditive(named:on:lookingAlong:orientationWeight:)

Creates a constraint with only an orientational demand in additive look-at mode.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
static func lookAtAdditive(
    named name: String,
    on jointName: String,
    lookingAlong targetAxis: SIMD3,
    orientationWeight: SIMD3 = [1, 1, 1]
) -> IKRig.Constraint
```

## Parameters 

`name`  

The rig unique name of the constraint

`jointName`  

The name of the joint to constrain.

`targetAxis`  

The axis from the constrained joint to look-at target position in the local space of the joint.

`orientationWeight`  

The weight of the orientation demand.

## Discussion

See Also

`IKOrientationDemand.Mode.additiveLookAt`

