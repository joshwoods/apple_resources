

- RealityKit
- IKRig
- 
  - IKRig
- IKRig.Constraint
- IKRig.Constraint.IKOrientationDemand
- IKRig.Constraint.IKOrientationDemand.Mode
-  IKRig.Constraint.IKOrientationDemand.Mode.additiveLookAt(targetAxis:) 

Case

# IKRig.Constraint.IKOrientationDemand.Mode.additiveLookAt(targetAxis:)

A mode which computes the rotation target as additive look-at.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
case additiveLookAt(targetAxis: SIMD3)
```

## Parameters 

`targetAxis`  

The unit vector from the joint to the look-at target defined in the local space of the constrained joint.

### Demand target

Source  
The model space orientation of the constrained joint from the FK demands pose.

Target  
The model space orientation aligning the associated `targetAxis` with the direction from the current model space joint position to lookAtTargetPosition.

Delta  
The rotation difference between `Source` and `Target`.

The rotation weight of animationOverrideWeight determines how much of the `Delta` is added to the `Source`.

