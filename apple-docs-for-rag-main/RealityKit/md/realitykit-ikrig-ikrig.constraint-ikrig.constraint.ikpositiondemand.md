

- RealityKit
- IKRig
- IKRig.Constraint
-  IKRig.Constraint.IKPositionDemand 

Structure

# IKRig.Constraint.IKPositionDemand

A definition of a positional demand.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct IKPositionDemand
```

## Topics

### Initializers

init()

Creates a positional demand with default settings.

### Instance Properties

var influenceDepthMaxJointCount: Int

The number of joints to be influenced by this demand.

var mode: IKRig.Constraint.IKPositionDemand.Mode

The mode of the positional demand.

var weight: SIMD3&lt;Float>

The per-axis weight this demand has on the pose.

### Enumerations

enum Mode

Describes the acting modes of positional demands.

