

- RealityKit
- IKComponent
-  IKComponent.Constraint 

Class

# IKComponent.Constraint

The update stage object that lets you read and update the current settings of a single constraint in an IK solver.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
class Constraint
```

## Overview

The settings this object exposes are the runtime editable values of the solver constraint. Initial values are set in IKRig.Constraint.

## Topics

### Structures

struct DemandOptions

Flags for the different demands types that can be active in a single constraint.

### Instance Properties

var animationOverrideWeight: (position: Float, rotation: Float)

The blending weights between the FK demand and the your target per demand type.

var demands: IKComponent.Constraint.DemandOptions

The set of the active demands of the constraint.

let id: IKComponent.Constraint.ID

ID of the constraint, that is unique within the solver instance.

var jointID: IKComponent.Joint.ID

The identifier of the constrained rig joint.

var lookAtTargetPosition: SIMD3&lt;Float>

The point demand which the look-at constraint uses to generate a new orientation demand.

var name: String

The name of the constraint as defined in the rig.

var offset: Transform

The offset applied on top of the target transform before the solve.

var target: Transform

The packed targets for the positional and orientational demands in model space.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

## Relationships

### Conforms To

- Identifiable

## See Also

### Inverse kinematics components

struct IKComponent

A component that allows you to procedurally animate a skeletal model using a full body inverse kinematics solver.

class Joint

The update stage object that lets you read and update the current settings of a single joint in an IK solver.

struct JointCollection

Ordered dictionary like container with fixed size.

class Solver

The update stage object that lets you read and update the current settings of a single solver instance.

struct SolverCollection

Ordered dictionary like container with fixed size.

struct ConstraintCollection

Ordered dictionary like container with fixed size.

class IKResource

A reference counted immutable resource which contains one or more inverse kinematics solver rigs.

struct IKSolverDefinition

A container describing a solver instance.

typealias ID

A type representing the stable identity of the entity associated with an instance.

