

- RealityKit
-  IKRig 

Structure

# IKRig

A full body inverse kinematics rig definition for a single skeleton.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct IKRig
```

## Overview

Describes the skeleton, its tuning, and the active constraints for the solver instance.

### Balance of demands’ weights in a full body solver

The full body solver calculates the final pose by balancing the various demands based on their assigned weights. This process ensures that each demand, ranging from forward kinematics (FK) demands to constraints on joint movement, affects the pose proportionally to its importance.

The solver reads the FK demands from the SkeletalPosesComponent. As such these demands are either a playing animation for the model, or just a static pose.

All demands have an element specific weight, and some have a global rig weight. The rig weights influence the overall rig, while element weights adjust individual aspects of the model.

The table below provides detailed mappings of these weights to their respective demand types.

| Demand type | Rig weight | Element weight |
|----|----|----|
| FK demands | globalFkWeight | fkWeightPerAxis |
| Joint rotation limits | globalLimitsWeight | weight |
| Constraint position | Not applicable | weight |
| Constraint orientation | Not applicable | weight |

Note

While constraints do not have rig weight, they have blending weight between automatic and custom targets. See animationOverrideWeight for more information.

## Topics

### Structures

struct Constraint

A definition of a rig constraint.

struct ConstraintsCollection

Ordered dictionary-like container.

struct Joint

A definition of a rig joint and its IK solver settings.

struct JointCollection

Ordered dictionary-like container with a fixed size.

### Initializers

init(for: MeshResource.Skeleton) throws

Creates an inverse kinematics rig definition for the provided skeleton.

### Instance Properties

var constraints: IKRig.ConstraintsCollection

A collection of all of the rig’s constraint settings.

var globalFkWeight: Float

The solver global weight for the forward kinematics demands.

var globalLimitsWeight: Float

The solver global weight for the joint rotation limits.

var joints: IKRig.JointCollection

A collection of all of the rig’s joint settings.

var maxIterations: Int

The maximum number of iterations the solver is allowed to do per frame.

## See Also

### Inverse kinematics rigs

struct Joint

A definition of a rig joint and its IK solver settings.

struct JointCollection

Ordered dictionary-like container with a fixed size.

struct Constraint

A definition of a rig constraint.

struct ConstraintsCollection

Ordered dictionary-like container.

