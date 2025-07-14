

- RealityKit
- IKRig
- IKRig.Constraint
-  IKRig.Constraint.IKOrientationDemand 

Structure

# IKRig.Constraint.IKOrientationDemand

A definition of an orientational demand.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct IKOrientationDemand
```

## Topics

### Initializers

init()

Creates an orientational demand with default settings.

### Instance Properties

var influenceDepthMaxJointCount: Int

The number of joints to be influenced by this demand.

var mode: IKRig.Constraint.IKOrientationDemand.Mode

The mode of the orientational demand.

var weight: SIMD3&lt;Float>

The per-axis weight this demand has on the pose.

### Enumerations

enum Mode

Describes the acting modes of an orientation demand.

