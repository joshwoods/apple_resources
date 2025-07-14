

- RealityKit
-  AnimationState 

Structure

# AnimationState

The concretely typed animation state structure.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct AnimationState where Value : AnimatableData
```

## Overview

Access the animation state structure from the event structure returned to the action’s `.updated` event handler. Define a valid bind target and matching animation type for the action animation to make the state structure available and non-nil.

(See: AnimationStateProtocol)

## Topics

### Instance Properties

var defaultSource: Value?

See: defaultSource

var defaultSource: JointTransforms?

Returns the joint transforms representing the default source value.

var defaultTarget: JointTransforms?

Returns the joint transforms representing the default target value.

var defaultTarget: Value?

See: defaultTarget

let deltaTime: TimeInterval

See: deltaTime

let evaluationTime: TimeInterval

See evaluationTime

let normalizedTime: TimeInterval

See normalizedTime

### Instance Methods

func defaultSourceJoints(index: Int, count: Int, transforms: inout [Transform]) -> Bool

Retrieves a subset of default source joints, and stores them in the output transform array.

func defaultTargetJoints(index: Int, count: Int, transforms: inout [Transform]) -> Bool

Retrieves a subset of default target joints, and stores them in the output transform array.

func storeAnimatedJoints(transforms: [Transform], jointIndex: Int) -> Bool

Stores a subset of animated joints.

func storeAnimatedValue&lt;ValueType>(ValueType) -> Bool

See: storeAnimatedValue(_:)

### Type Aliases

typealias ValueType

## Relationships

### Conforms To

- AnimationStateProtocol

## See Also

### Action events

struct ActionEvent

The structure returned to all action event handlers.

struct ActionEventType

A set of events that an action responds to.

struct ActionEventDefinition

Defines an action event interval, and any associated parameters.

protocol AnimationStateProtocol

The protocol representing the current animation state of an action animation.

