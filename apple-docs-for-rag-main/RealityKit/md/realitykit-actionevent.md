

- RealityKit
-  ActionEvent 

Structure

# ActionEvent

The structure returned to all action event handlers.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct ActionEvent where ActionType : EntityAction
```

## Overview

Actions perform their function within one or more custom event handlers associated with an action type.

The event structure contains useful information for an action to perform its function when an action event is raised.

## Topics

### Instance Properties

let action: ActionType

The action parameter data that remains constant across one or more events intervals defined for the action animation.

var animationState: (any AnimationStateProtocol)?

The animation state for the action.

let duration: TimeInterval

The duration of the the event.

let parameter: ActionType.EventParameterType?

The event parameter data that can vary for each event.

let playbackController: AnimationPlaybackController

The animation playback controller that manages the animation executing the action.

let reversed: Bool

A Boolean value that indicates reverse playback when true.

let startTime: TimeInterval

The start time of the current event.

let targetEntity: Entity?

The entity the bind target references.

## See Also

### Action events

struct AnimationState

The concretely typed animation state structure.

struct ActionEventType

A set of events that an action responds to.

struct ActionEventDefinition

Defines an action event interval, and any associated parameters.

protocol AnimationStateProtocol

The protocol representing the current animation state of an action animation.

