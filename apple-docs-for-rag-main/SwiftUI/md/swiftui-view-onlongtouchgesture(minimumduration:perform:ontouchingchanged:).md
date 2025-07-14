

- SwiftUI
- View
-  onLongTouchGesture(minimumDuration:perform:onTouchingChanged:) 

Instance Method

# onLongTouchGesture(minimumDuration:perform:onTouchingChanged:)

Adds an action to perform when this view recognizes a remote long touch gesture. A long touch gesture is when the finger is on the remote touch surface without actually pressing.

tvOS 16.0+

``` source
nonisolated
func onLongTouchGesture(
    minimumDuration: Double = 0.5,
    perform action: @escaping () -> Void,
    onTouchingChanged: ((Bool) -> Void)? = nil
) -> some View
```

## Parameters 

`minimumDuration`  

The minimum duration of the long touch that must elapse before the gesture succeeds.

`action`  

The action to perform when a long touch is recognized

`onTouchingChanged`  

A closure to run when the touching state of the gesture changes, passing the current state as a parameter.

## See Also

### Recognizing long press gestures

func onLongPressGesture(minimumDuration: Double, maximumDistance: CGFloat, perform: () -> Void, onPressingChanged: ((Bool) -> Void)?) -> some View

Adds an action to perform when this view recognizes a long press gesture.

func onLongPressGesture(minimumDuration: Double, perform: () -> Void, onPressingChanged: ((Bool) -> Void)?) -> some View

Adds an action to perform when this view recognizes a long press gesture.

struct LongPressGesture

A gesture that succeeds when the user performs a long press.

