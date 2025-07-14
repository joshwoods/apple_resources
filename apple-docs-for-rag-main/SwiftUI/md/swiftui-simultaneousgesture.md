

- SwiftUI
-  SimultaneousGesture 

Structure

# SimultaneousGesture

A gesture containing two gestures that can happen at the same time with neither of them preceding the other.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct SimultaneousGesture where First : Gesture, Second : Gesture
```

## Overview

A simultaneous gesture is a container-event handler that evaluates its two child gestures at the same time. Its value is a struct with two optional values, each representing the phases of one of the two gestures.

## Topics

### Creating the gesture

init(First, Second)

Creates a gesture with two gestures that can receive updates or succeed independently of each other.

var first: First

The first of two gestures that can happen simultaneously.

var second: Second

The second of two gestures that can happen simultaneously.

### Getting the gesture’s values

struct Value

The value of a simultaneous gesture that indicates which of its two gestures receives events.

## Relationships

### Conforms To

- Gesture

## See Also

### Combining gestures

Composing SwiftUI gestures

Combine gestures to create complex interactions.

func simultaneousGesture&lt;T>(T, including: GestureMask) -> some View

Attaches a gesture to the view to process simultaneously with gestures defined by the view.

func simultaneousGesture&lt;T>(T, isEnabled: Bool) -> some View

Attaches a gesture to the view to process simultaneously with gestures defined by the view.

func simultaneousGesture&lt;T>(T, name: String, isEnabled: Bool) -> some View

Attaches a gesture to the view to process simultaneously with gestures defined by the view.

struct SequenceGesture

A gesture that’s a sequence of two gestures.

struct ExclusiveGesture

A gesture that consists of two gestures where only one of them can succeed.

