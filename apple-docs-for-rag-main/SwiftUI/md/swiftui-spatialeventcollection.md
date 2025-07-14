

- SwiftUI
-  SpatialEventCollection 

Structure

# SpatialEventCollection

A collection of spatial input events that target a specific view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+watchOS 11.0+

``` source
struct SpatialEventCollection
```

## Overview

You receive a structure of this type as an input to the onChanged(_:) or onEnded(_:) method of a SpatialEventGesture. The structure contains a collection of SpatialEventCollection.Event values that correspond to ongoing input events. You can look up a specific event in the collection by its id value or iterate over all events in the collection to apply logic depending on the event’s state.

## Topics

### Accessing the collection’s events

struct Event

A spatial event generated from an input like a touch or click that can drive gestures in the system.

subscript(SpatialEventCollection.Event.ID) -> SpatialEventCollection.Event?

Retrieves an event using its unique identifier.

### Iterating over events in the collection

func makeIterator() -> SpatialEventCollection.Iterator

Makes an iterator over all events in the collection.

struct Iterator

An iterator over all events in the collection.

## Relationships

### Conforms To

- Collection
- Copyable
- Equatable
- Sequence

## See Also

### Recognizing spatial events

struct SpatialEventGesture

A gesture that provides information about ongoing spatial events like clicks and touches.

enum Chirality

The chirality, or handedness, of a pose.

