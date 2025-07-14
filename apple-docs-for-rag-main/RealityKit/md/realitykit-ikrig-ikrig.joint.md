

- RealityKit
- IKRig
-  IKRig.Joint 

Structure

# IKRig.Joint

A definition of a rig joint and its IK solver settings.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct Joint
```

## Topics

### Structures

struct ID

The identity type for a joint in a rig.

struct LimitsDefinition

A definition of joint rotation limits.

### Initializers

init(name: String, parentID: IKRig.Joint.ID?, restTransform: Transform)

Creates a joint with the provided base elements.

### Instance Properties

var active: Bool

A boolean value that sets whether the solver rotates the joint.

var fkWeightPerAxis: SIMD3&lt;Float>

The per-axis weight of the FK demand on the joint.

var id: IKRig.Joint.ID

The identifier of the joint.

var limits: IKRig.Joint.LimitsDefinition?

The per-axis rotation limits of the joint.

let name: String

The name of the joint.

var parentID: IKRig.Joint.ID?

The identifier of the parent joint if there is one.

var restTransform: Transform

The local space transformation of the joint in the solver’s rest pose.

var rotationStiffness: SIMD3&lt;Float>

The per-axis rotational stiffness of the joint.

## Relationships

### Conforms To

- Identifiable

## See Also

### Inverse kinematics rigs

struct IKRig

A full body inverse kinematics rig definition for a single skeleton.

struct JointCollection

Ordered dictionary-like container with a fixed size.

struct Constraint

A definition of a rig constraint.

struct ConstraintsCollection

Ordered dictionary-like container.

