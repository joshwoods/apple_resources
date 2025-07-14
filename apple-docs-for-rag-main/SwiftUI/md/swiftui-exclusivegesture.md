

- SwiftUI
-  ExclusiveGesture 

Structure

# ExclusiveGesture

A gesture that consists of two gestures where only one of them can succeed.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct ExclusiveGesture where First : Gesture, Second : Gesture
```

## Overview

The `ExclusiveGesture` gives precedence to its first gesture.

## Topics

### Creating the gesture

init(First, Second)

Creates a gesture from two gestures where only one of them succeeds.

var first: First

The first of two gestures.

var second: Second

The second of two gestures.

### Supporting types

enum Value

The value of an exclusive gesture that indicates which of two gestures succeeded.

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

struct SimultaneousGesture

A gesture containing two gestures that can happen at the same time with neither of them preceding the other.

