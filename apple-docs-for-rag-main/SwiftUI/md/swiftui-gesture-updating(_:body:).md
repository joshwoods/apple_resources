

- SwiftUI
- Gesture
-  updating(\_:body:) 

Instance Method

# updating(\_:body:)

Updates the provided gesture state property as the gesture’s value changes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @preconcurrency
func updating(
    _ state: GestureState,
    body: @escaping (Self.Value, inout State, inout Transaction) -> Void
) -> GestureStateGesture
```

## Parameters 

`state`  

A binding to a view’s GestureState property.

`body`  

The callback that SwiftUI invokes as the gesture’s value changes. Its `currentState` parameter is the updated state of the gesture. The `gestureState` parameter is the previous state of the gesture, and the `transaction` is the context of the gesture.

## Return Value

A version of the gesture that updates the provided `state` as the originating gesture’s value changes and that resets the `state` to its initial value when the user or the system ends or cancels the gesture.

## Mentioned in 

Adding interactivity with gestures

## Discussion

Use this callback to update transient UI state as described in Adding interactivity with gestures.

## See Also

### Performing the gesture

func onChanged((Self.Value) -> Void) -> _ChangedGesture&lt;Self>

Adds an action to perform when the gesture’s value changes.

func onEnded((Self.Value) -> Void) -> _EndedGesture&lt;Self>

Adds an action to perform when the gesture ends.

associatedtype Value

The type representing the gesture’s value.

**Required**

