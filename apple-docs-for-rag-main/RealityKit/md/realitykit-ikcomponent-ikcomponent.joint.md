

- RealityKit
- IKComponent
-  IKComponent.Joint 

Class

# IKComponent.Joint

The update stage object that lets you read and update the current settings of a single joint in an IK solver.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
class Joint
```

## Overview

The settings this object exposes are the runtime editable values of a solver joint. Initial values are set in IKRig.Joint.

## Topics

### Instance Properties

var fkWeightPerAxis: SIMD3&lt;Float>

The per-axis weight of the source animation demand on the joint.

let id: IKComponent.Joint.ID

The identifier of this joint.

var name: String

The name of the joint.

var rotationStiffness: SIMD3&lt;Float>

The per-axis rotational stiffness of the joint.

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

struct JointCollection

Ordered dictionary like container with fixed size.

class Solver

The update stage object that lets you read and update the current settings of a single solver instance.

struct SolverCollection

Ordered dictionary like container with fixed size.

class Constraint

The update stage object that lets you read and update the current settings of a single constraint in an IK solver.

struct ConstraintCollection

Ordered dictionary like container with fixed size.

class IKResource

A reference counted immutable resource which contains one or more inverse kinematics solver rigs.

struct IKSolverDefinition

A container describing a solver instance.

typealias ID

A type representing the stable identity of the entity associated with an instance.

