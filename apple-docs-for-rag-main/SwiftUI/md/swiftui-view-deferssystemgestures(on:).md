

- SwiftUI
- View
-  defersSystemGestures(on:) 

Instance Method

# defersSystemGestures(on:)

Sets the screen edge from which you want your gesture to take precedence over the system gesture.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
nonisolated
func defersSystemGestures(on edges: Edge.Set) -> some View
```

## Parameters 

`edges`  

A value that indicates the screen edge from which you want your gesture to take precedence over the system gesture.

## Discussion

The following code defers the vertical screen edges system gestures of a given canvas.

```
struct DeferredView: View {
    var body: some View {
        Canvas()
            .defersSystemGestures(on: .vertical)
    }
}
```

## See Also

### Defining custom gestures

func highPriorityGesture&lt;T>(T, including: GestureMask) -> some View

Attaches a gesture to the view with a higher precedence than gestures defined by the view.

func highPriorityGesture&lt;T>(T, isEnabled: Bool) -> some View

Attaches a gesture to the view with a higher precedence than gestures defined by the view.

func highPriorityGesture&lt;T>(T, name: String, isEnabled: Bool) -> some View

Attaches a gesture to the view with a higher precedence than gestures defined by the view.

func handGestureShortcut(HandGestureShortcut, isEnabled: Bool) -> some View

Assigns a hand gesture shortcut to the modified control.

protocol Gesture

An instance that matches a sequence of events to a gesture, and returns a stream of values for each of its states.

struct AnyGesture

A type-erased gesture.

struct HandActivationBehavior

An activation behavior specific to hand-driven input.

struct HandGestureShortcut

Hand gesture shortcuts describe finger and wrist movements that the user can perform in order to activate a button or toggle.

