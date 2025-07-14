

- RealityKit
- IKRig
-  IKRig.Constraint 

Structure

# IKRig.Constraint

A definition of a rig constraint.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct Constraint
```

## Overview

Each constraint can have its position and orientation demands enabled individually.

## Topics

### Structures

struct ID

The identity type for a constraint in a rig.

struct IKOrientationDemand

A definition of an orientational demand.

struct IKPositionDemand

A definition of a positional demand.

### Instance Properties

var id: IKRig.Constraint.ID

The identifier of the constraint.

var jointName: String

The name of the constrained joint.

var name: String

The name of the constraint.

var offset: Transform

A constraint target offset.

var orientationDemand: IKRig.Constraint.IKOrientationDemand?

The settings of the orientational demand.

var positionDemand: IKRig.Constraint.IKPositionDemand?

The settings of the positional demand.

### Type Methods

static func lookAtAbsolute(named: String, on: String, lookingAlong: SIMD3&lt;Float>, orientationWeight: SIMD3&lt;Float>) -> IKRig.Constraint

Creates a constraint with only an orientational demand in absolute look-at mode.

static func lookAtAdditive(named: String, on: String, lookingAlong: SIMD3&lt;Float>, orientationWeight: SIMD3&lt;Float>) -> IKRig.Constraint

Creates a constraint with only an orientational demand in additive look-at mode.

static func orient(named: String, on: String, orientationWeight: SIMD3&lt;Float>) -> IKRig.Constraint

Creates a constraint with only an orientation demand.

static func parent(named: String, on: String, positionWeight: SIMD3&lt;Float>, orientationWeight: SIMD3&lt;Float>) -> IKRig.Constraint

Creates a constraint with both a positional and an orientational demands.

static func point(named: String, on: String, positionWeight: SIMD3&lt;Float>) -> IKRig.Constraint

Creates a constraint with only a positional demand.

## Relationships

### Conforms To

- Identifiable

## See Also

### Inverse kinematics rigs

struct IKRig

A full body inverse kinematics rig definition for a single skeleton.

struct Joint

A definition of a rig joint and its IK solver settings.

struct JointCollection

Ordered dictionary-like container with a fixed size.

struct ConstraintsCollection

Ordered dictionary-like container.

