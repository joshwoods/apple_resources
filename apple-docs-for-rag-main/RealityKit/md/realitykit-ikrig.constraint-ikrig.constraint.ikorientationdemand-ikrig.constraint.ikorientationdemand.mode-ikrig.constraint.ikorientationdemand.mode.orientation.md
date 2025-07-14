

- RealityKit
- IKRig
- 
  - IKRig
- IKRig.Constraint
- IKRig.Constraint.IKOrientationDemand
- IKRig.Constraint.IKOrientationDemand.Mode
-  IKRig.Constraint.IKOrientationDemand.Mode.orientation 

Case

# IKRig.Constraint.IKOrientationDemand.Mode.orientation

A mode which uses the set rotation target.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
case orientation
```

### Demand target

Source  
The model space orientation of the constrained joint from the FK demands pose.

Target  
The rotation component of target.

The rotation weight of animationOverrideWeight determines how the rotation target is calculated:

- A weight of **`0`** uses the `Source`.

- A weight of **`1`** uses the `Target`.

- A weight **between `0` and `1`** results in a spherical linear interpolation between the `Source` and `Target`.

