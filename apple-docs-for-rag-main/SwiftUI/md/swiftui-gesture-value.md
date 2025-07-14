

- SwiftUI
- Gesture
-  Value 

Associated Type

# Value

The type representing the gesture’s value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
associatedtype Value
```

**Required**

## See Also

### Performing the gesture

func updating&lt;State>(GestureState&lt;State>, body: (Self.Value, inout State, inout Transaction) -> Void) -> GestureStateGesture&lt;Self, State>

Updates the provided gesture state property as the gesture’s value changes.

func onChanged((Self.Value) -> Void) -> _ChangedGesture&lt;Self>

Adds an action to perform when the gesture’s value changes.

func onEnded((Self.Value) -> Void) -> _EndedGesture&lt;Self>

Adds an action to perform when the gesture ends.

