

- RealityKit
-  ActionEventType 

Structure

# ActionEventType

A set of events that an action responds to.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct ActionEventType
```

## Overview

Actions can respond to specific events with one or more custom event handlers that you associate with each event type.

RealityKit calls the event handlers when the animation time enters, exits, or continues within a time interval for an ActionEventDefinition.

A time interval for an event begins at its starting time and spans up to, but doesn’t include, the event’s starting time plus its duration.

## Topics

### Event types

static var started: ActionEventType

An event that takes place when a new action event begins.

static var ended: ActionEventType

An event that takes place when the action event exits its time interval.

static var paused: ActionEventType

An event that takes place when the animation pauses.

static var resumed: ActionEventType

An event that takes place when the animation resumes after a pause.

static var updated: ActionEventType

An event that takes place after an action event starts and is within its time interval.

static var skipped: ActionEventType

An event that takes place when the system misses an action event’s time interval.

static var terminated: ActionEventType

An event that takes place when the animation ends.

### Protocol support

init(rawValue: UInt)

Creates an action event type from a raw value.

let rawValue: UInt

The backing storage for action event types.

typealias ArrayLiteralElement

The type of the elements of an array literal.

typealias Element

The element type of the option set.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

Equatable Implementations

OptionSet Implementations

RawRepresentable Implementations

SetAlgebra Implementations

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- Hashable
- OptionSet
- RawRepresentable
- SetAlgebra

## See Also

### Action events

struct ActionEvent

The structure returned to all action event handlers.

struct AnimationState

The concretely typed animation state structure.

struct ActionEventDefinition

Defines an action event interval, and any associated parameters.

protocol AnimationStateProtocol

The protocol representing the current animation state of an action animation.

