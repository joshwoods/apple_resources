

- RealityKit
-  ActionEventDefinition 

Structure

# ActionEventDefinition

Defines an action event interval, and any associated parameters.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct ActionEventDefinition where ActionType : EntityAction
```

## Overview

Start, update, end, and skipped events are raised based on one or more event intervals defined by the action animation.

Also see: ActionEventType

## Topics

### Initializers

init(startTime: TimeInterval, duration: TimeInterval, parameter: ActionEventDefinition&lt;ActionType>.EventParameterType?)

Constructs an event definition.

### Instance Properties

var duration: TimeInterval

The event interval’s duration.

var parameter: ActionEventDefinition&lt;ActionType>.EventParameterType?

Optional parameter data available to the event handler at the time of the event.

var startTime: TimeInterval

The time at which the event interval starts.

### Type Aliases

typealias EventParameterType

## See Also

### Action events

struct ActionEvent

The structure returned to all action event handlers.

struct AnimationState

The concretely typed animation state structure.

struct ActionEventType

A set of events that an action responds to.

protocol AnimationStateProtocol

The protocol representing the current animation state of an action animation.

