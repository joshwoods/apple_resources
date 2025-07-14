

- RealityKit
- IKComponent
-  IKComponent.Solver 

Class

# IKComponent.Solver

The update stage object that lets you read and update the current settings of a single solver instance.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
class Solver
```

## Overview

The settings this object exposes are the runtime editable values on the solver instance itself, the solver joints and constraints. For the full list of settings adjustable during creation, see IKRig.

## Topics

### Structures

struct ID

The solver instance identifier type.

### Instance Properties

var constraints: IKComponent.ConstraintCollection

The collection of all of the constraint update stage objects of the solver instance.

var globalFkWeight: Float

The solver global forward kinematics demand’s weight.

var id: IKComponent.Solver.ID

The solver instance identifier.

var joints: IKComponent.JointCollection

The collection of all of the joint update stage objects of the solver instance.

var maxIterations: Int

The maximum number of iterations the solver is allowed to do per frame.

### Instance Methods

func reset()

Enqueues a solver reset call that executes before the next solve.

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

