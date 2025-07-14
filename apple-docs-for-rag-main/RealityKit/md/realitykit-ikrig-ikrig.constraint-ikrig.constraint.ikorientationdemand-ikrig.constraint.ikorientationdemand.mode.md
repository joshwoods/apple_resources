

- RealityKit
- IKRig
- IKRig.Constraint
- IKRig.Constraint.IKOrientationDemand
-  IKRig.Constraint.IKOrientationDemand.Mode 

Enumeration

# IKRig.Constraint.IKOrientationDemand.Mode

Describes the acting modes of an orientation demand.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
enum Mode
```

## Topics

### Enumeration Cases

case absoluteLookAt(targetAxis: SIMD3&lt;Float>)

A mode which computes the rotation target as absolute look-at.

case additiveLookAt(targetAxis: SIMD3&lt;Float>)

A mode which computes the rotation target as additive look-at.

case orientation

A mode which uses the set rotation target.

