

- RealityKit
-  IKResource 

Class

# IKResource

A reference counted immutable resource which contains one or more inverse kinematics solver rigs.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
class IKResource
```

## Overview

Use this resource with an IKComponent.

## Topics

### Initializers

convenience init(rig: IKRig) throws

Creates a new resource instance for a single solver using the given rig and an automatic solver identifier.

### Instance Properties

var solverDefinitions: [IKSolverDefinition]

Getter for the deserialized resource contents as a collection of solver definitions.

## Relationships

### Conforms To

- Resource
- Sendable

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

struct IKSolverDefinition

A container describing a solver instance.

typealias ID

A type representing the stable identity of the entity associated with an instance.

