

- RealityKit
- IKRig
- 
  - IKRig
- IKRig.Constraint
- IKRig.Constraint.IKOrientationDemand
- IKRig.Constraint.IKOrientationDemand.Mode
-  IKRig.Constraint.IKOrientationDemand.Mode.absoluteLookAt(targetAxis:) 

Case

# IKRig.Constraint.IKOrientationDemand.Mode.absoluteLookAt(targetAxis:)

A mode which computes the rotation target as absolute look-at.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
case absoluteLookAt(targetAxis: SIMD3)
```

## Parameters 

`targetAxis`  

The unit vector from the joint to the look-at target defined in the model space of the entity.

### Demand target

Source  
The model space orientation of the constrained joint from the FK demands pose.

Target  
The model space orientation aligning the associated `targetAxis` with the direction from the current model space joint position to lookAtTargetPosition.

The rotation weight of animationOverrideWeight determines how the rotation target is calculated:

- A weight of **`0`** uses the `Source`.

- A weight of **`1`** uses the `Target`.

- A weight **between `0` and `1`** results in a spherical linear interpolation between the `Source` and `Target`.

