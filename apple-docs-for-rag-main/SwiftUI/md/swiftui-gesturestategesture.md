

- SwiftUI
-  GestureStateGesture 

Structure

# GestureStateGesture

A gesture that updates the state provided by a gesture’s updating callback.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct GestureStateGesture where Base : Gesture
```

## Overview

A gesture’s updating(_:body:) callback returns a `GestureStateGesture` instance for updating a transient state property that’s annotated with the GestureState property wrapper.

## Topics

### Creating an in-progress gesture

init(base: Base, state: GestureState&lt;State>, body: (GestureStateGesture&lt;Base, State>.Value, inout State, inout Transaction) -> Void)

Creates a new gesture that’s the result of an ongoing gesture.

var base: Base

The originating gesture.

var state: GestureState&lt;State>

A value that changes as the user performs the gesture.

### Supporting types

var body: (GestureStateGesture&lt;Base, State>.Value, inout State, inout Transaction) -> Void

The updating gesture containing the originating gesture’s value, the updated state of the gesture, and a transaction.

## Relationships

### Conforms To

- Gesture

## See Also

### Managing gesture state

struct GestureState

A property wrapper type that updates a property while the user performs a gesture and resets the property back to its initial state when the gesture ends.

