

- SwiftUI
- Gesture
-  onChanged(\_:) 

Instance Method

# onChanged(\_:)

Adds an action to perform when the gesture’s value changes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @preconcurrency
func onChanged(_ action: @escaping (Self.Value) -> Void) -> _ChangedGesture
```

Available when `Value` conforms to `Equatable`.

## Parameters 

`action`  

The action to perform when this gesture’s value changes. The `action` closure’s parameter contains the gesture’s new value.

## Return Value

A gesture that triggers `action` when this gesture’s value changes.

## Mentioned in 

Adding interactivity with gestures

## See Also

### Performing the gesture

func updating&lt;State>(GestureState&lt;State>, body: (Self.Value, inout State, inout Transaction) -> Void) -> GestureStateGesture&lt;Self, State>

Updates the provided gesture state property as the gesture’s value changes.

func onEnded((Self.Value) -> Void) -> _EndedGesture&lt;Self>

Adds an action to perform when the gesture ends.

associatedtype Value

The type representing the gesture’s value.

**Required**

