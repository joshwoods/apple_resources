

- SwiftUI
-  SequenceGesture 

Structure

# SequenceGesture

A gesture that’s a sequence of two gestures.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct SequenceGesture where First : Gesture, Second : Gesture
```

## Overview

Read Composing SwiftUI gestures to learn how you can create a sequence of two gestures.

## Topics

### Creating the gesture

init(First, Second)

Creates a sequence gesture with two gestures.

var first: First

The first gesture in a sequence of two gestures.

var second: Second

The second gesture in a sequence of two gestures.

### Getting the gesture’s values

enum Value

The value of a sequence gesture that helps to detect whether the first gesture succeeded, so the second gesture can start.

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

struct SimultaneousGesture

A gesture containing two gestures that can happen at the same time with neither of them preceding the other.

struct ExclusiveGesture

A gesture that consists of two gestures where only one of them can succeed.

