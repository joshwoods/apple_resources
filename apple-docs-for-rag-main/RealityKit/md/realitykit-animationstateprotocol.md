

- RealityKit
-  AnimationStateProtocol 

Protocol

# AnimationStateProtocol

The protocol representing the current animation state of an action animation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
protocol AnimationStateProtocol
```

## Overview

The animation state allows actions to animate a target value using RealityKit’s animation engine.

Animating values with the animation engine allows for cross-fading and additive compositing with other RealityKit animations targeting the same value.

Access the animation state structure from the event structure returned to `.updated` event handlers. Define a valid bind target and matching animation type to make the state structure available and non nil.

Note

Custom actions don’t support animating BlendShapeWeights.

## Topics

### Associated Types

associatedtype ValueType : AnimatableData

**Required**

### Instance Properties

var defaultSource: Self.ValueType?

The previous blend stage value.

**Required**

var defaultTarget: Self.ValueType?

The default unanimated value of the target.

**Required**

var deltaTime: TimeInterval

The time that has elapsed since the most recent evaluation, or 0 if animation is paused.

**Required**

var evaluationTime: TimeInterval

The time at which the animation result should be evaluated.

**Required**

var normalizedTime: TimeInterval

The normalized time ranges from 0 to 1, and is the time at which the animation result should be evaluated.

**Required**

### Instance Methods

func storeAnimatedValue&lt;ValueType>(ValueType) -> Bool

Stores the action’s animated value, which the animation manager uses to produce a final animated result. Returns true on success, otherwise false.

**Required**

## Relationships

### Conforming Types

- AnimationState

## See Also

### Action events

struct ActionEvent

The structure returned to all action event handlers.

struct AnimationState

The concretely typed animation state structure.

struct ActionEventType

A set of events that an action responds to.

struct ActionEventDefinition

Defines an action event interval, and any associated parameters.

