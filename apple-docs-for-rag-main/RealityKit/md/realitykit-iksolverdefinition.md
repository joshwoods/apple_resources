

- RealityKit
-  IKSolverDefinition 

Structure

# IKSolverDefinition

A container describing a solver instance.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct IKSolverDefinition
```

## Overview

Adds unique identifier for each solver instance as the rig can be reused.

## Topics

### Initializers

init(id: IKSolverDefinition.ID, rig: IKRig)

Creates a solver definition for with a unique solver identifier and a rig.

### Instance Properties

let id: IKSolverDefinition.ID

The identifier of the solver instance.

var rigDefinition: IKRig

The solver’s rig definition.

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

class Constraint

The update stage object that lets you read and update the current settings of a single constraint in an IK solver.

struct ConstraintCollection

Ordered dictionary like container with fixed size.

class IKResource

A reference counted immutable resource which contains one or more inverse kinematics solver rigs.

typealias ID

A type representing the stable identity of the entity associated with an instance.

