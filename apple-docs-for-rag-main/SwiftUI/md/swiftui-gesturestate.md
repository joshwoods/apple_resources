

- SwiftUI
-  GestureState 

Structure

# GestureState

A property wrapper type that updates a property while the user performs a gesture and resets the property back to its initial state when the gesture ends.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@propertyWrapper @frozen
struct GestureState
```

## Mentioned in 

Adding interactivity with gestures

## Overview

Declare a property as `@GestureState`, pass as a binding to it as a parameter to a gesture’s updating(_:body:) callback, and receive updates to it. A property that’s declared as `@GestureState` implicitly resets when the gesture becomes inactive, making it suitable for tracking transient state.

Add a long-press gesture to a Circle, and update the interface during the gesture by declaring a property as `@GestureState`:

```
struct SimpleLongPressGestureView: View {
    @GestureState private var isDetectingLongPress = false

    var longPress: some Gesture {
        LongPressGesture(minimumDuration: 3)
            .updating($isDetectingLongPress) { currentState, gestureState, transaction in
                gestureState = currentState
            }
    }

    var body: some View {
        Circle()
            .fill(self.isDetectingLongPress ? Color.red : Color.green)
            .frame(width: 100, height: 100, alignment: .center)
            .gesture(longPress)
    }
}
```

## Topics

### Creating a gesture state

init(initialValue: Value)

Creates a view state that’s derived from a gesture with an initial value.

init(initialValue: Value, reset: (Value, inout Transaction) -> Void)

Creates a view state that’s derived from a gesture with an initial state value and a closure that provides a transaction to reset it.

init(initialValue: Value, resetTransaction: Transaction)

Creates a view state that’s derived from a gesture with an initial state value and a transaction to reset it.

init(reset: (Value, inout Transaction) -> Void)

Creates a view state that’s derived from a gesture with a closure that provides a transaction to reset it.

init(resetTransaction: Transaction)

Creates a view state that’s derived from a gesture with a transaction to reset it.

init(wrappedValue: Value)

Creates a view state that’s derived from a gesture.

init(wrappedValue: Value, reset: (Value, inout Transaction) -> Void)

Creates a view state that’s derived from a gesture with a wrapped state value and a closure that provides a transaction to reset it.

init(wrappedValue: Value, resetTransaction: Transaction)

Creates a view state that’s derived from a gesture with a wrapped state value and a transaction to reset it.

### Getting the state

var wrappedValue: Value

The wrapped value referenced by the gesture state property.

var projectedValue: GestureState&lt;Value>

A binding to the gesture state property.

## Relationships

### Conforms To

- DynamicProperty
- Sendable

## See Also

### Managing gesture state

struct GestureStateGesture

A gesture that updates the state provided by a gesture’s updating callback.

