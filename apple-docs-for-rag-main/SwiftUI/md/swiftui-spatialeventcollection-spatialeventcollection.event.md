

- SwiftUI
- SpatialEventCollection
-  SpatialEventCollection.Event 

Structure

# SpatialEventCollection.Event

A spatial event generated from an input like a touch or click that can drive gestures in the system.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+watchOS 11.0+

``` source
struct Event
```

## Overview

You receive a collection of these events in the form of a SpatialEventCollection that’s the input to the onChanged(_:) or onEnded(_:) method of a SpatialEventGesture. Inspect individual events to track interactions that enable you to create complex, multi-touch experiences in your app.

## Topics

### Identifying the event

var timestamp: TimeInterval

The time the event was processed.

var id: SpatialEventCollection.Event.ID

An identifier that uniquely identifies the event over its lifetime.

struct ID

A value that uniquely identifies an event over the course of its lifetime.

var kind: SpatialEventCollection.Event.Kind

The event’s input source.

enum Kind

The possible input sources or modes of an event.

var modifierKeys: EventModifiers

The set of active modifier keys at the time of this event.

### Locating the event

var location: CGPoint

The 2D location of the event.

var location3D: Point3D

The 3D location of the touch.

var selectionRay: Ray3D?

The 3D ray used to target the touch.

var inputDevicePose: SpatialEventCollection.Event.InputDevicePose?

The 3D position and orientation of the device controlling the touch, if one exists.

struct InputDevicePose

A pose describing the input device like a hand controlling the event.

var targetedEntity: Entity?

The entity target for this touch, if one exists.

### Getting the event’s current phase

var phase: SpatialEventCollection.Event.Phase

The phase of the event.

enum Phase

The states that an event can have.

### Instance Properties

var chirality: Chirality?

The hand chirality (left or right) of this event, for relevant event kinds.

## Relationships

### Conforms To

- Equatable
- Hashable
- Identifiable

## See Also

### Accessing the collection’s events

subscript(SpatialEventCollection.Event.ID) -> SpatialEventCollection.Event?

Retrieves an event using its unique identifier.

