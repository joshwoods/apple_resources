

- SwiftUI
- Gesture
-  onEnded(\_:) 

Instance Method

# onEnded(\_:)

Adds an action to perform when the gesture ends.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func onEnded(_ action: @escaping (Self.Value) -> Void) -> _EndedGesture
```

## Parameters 

`action`  

The action to perform when this gesture ends. The `action` closure’s parameter contains the final value of the gesture.

## Return Value

A gesture that triggers `action` when the gesture ends.

## Mentioned in 

Adding interactivity with gestures

## See Also

### Performing the gesture

func updating&lt;State>(GestureState&lt;State>, body: (Self.Value, inout State, inout Transaction) -> Void) -> GestureStateGesture&lt;Self, State>

Updates the provided gesture state property as the gesture’s value changes.

func onChanged((Self.Value) -> Void) -> _ChangedGesture&lt;Self>

Adds an action to perform when the gesture’s value changes.

associatedtype Value

The type representing the gesture’s value.

**Required**

