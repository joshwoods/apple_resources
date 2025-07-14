

- RealityKit
-  ActionAnimation 

Structure

# ActionAnimation

Defines an an action animation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct ActionAnimation where ActionType : EntityAction
```

## Overview

The definition is used to generate an action animation based `AnimationResource` that can then be played by calling playAnimation(_:transitionDuration:blendLayerOffset:separateAnimatedValue:startsPaused:clock:handoffType:)

Action animations can be used to perform operations in lock-step with playback.

Actions can be grouped or sequenced with pre-existing animation resources or be stand alone. For example an action that triggers sound can be grouped with a sampled animation to trigger sound effects at the appropriate times during playback. See: group(with:)

Stand alone action animations can animate target values using RealityKit’s animation engine with cross fade, and additive compositing support.

(See: AnimationStateProtocol)

## Topics

### Initializers

init(for: ActionType, events: [ActionAnimation&lt;ActionType>.EventDefinitionType], name: String, bindTarget: BindTarget?, blendLayer: Int32, repeatMode: AnimationRepeatMode, fillMode: AnimationFillMode, trimStart: TimeInterval?, trimEnd: TimeInterval?, trimDuration: TimeInterval?, offset: TimeInterval, delay: TimeInterval, speed: Float)

Constructs an action animation that generates events at user defined times.

### Instance Properties

var action: ActionType?

The action for which an animation is being defined.

var bindTarget: BindTarget

bindTarget is not used.

var blendLayer: Int32

blendLayer is not used.

var delay: TimeInterval

An amount of time that lapses before the animation plays.

var duration: TimeInterval

The elapsed time for one complete rotation.

var eventDefinitions: [ActionEventDefinition&lt;ActionType>]

The event interval definitions, and their associated parameter data.

var fillMode: AnimationFillMode

An option that determines which data displays outside of the normal duration.

var name: String

A textual name for the animation.

var offset: TimeInterval

The time, in seconds, at which the animation begins within the duration.

var repeatMode: AnimationRepeatMode

An option that determines how the animation repeats.

var speed: Float

A factor that changes the animation’s rate of playback.

var trimDuration: TimeInterval?

An optional duration that overrides the calculated duration.

var trimEnd: TimeInterval?

The optional time, in seconds, at which the animation stops.

var trimStart: TimeInterval?

The optional time, in seconds, at which the animation plays.

### Type Aliases

typealias EventDefinitionType

typealias EventParameterType

### Default Implementations

AnimationDefinition Implementations

## Relationships

### Conforms To

- AnimationDefinition

## See Also

### Action management

protocol EntityAction

A protocol that defines an action for an entity.

enum ActionEntityResolution

Options available to determine the resolution method for a target entity in an action.

protocol ActionHandlerProtocol

The base protocol for action handlers.

