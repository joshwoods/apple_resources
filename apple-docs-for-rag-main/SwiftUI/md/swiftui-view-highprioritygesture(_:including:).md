

- SwiftUI
- View
-  highPriorityGesture(\_:including:) 

Instance Method

# highPriorityGesture(\_:including:)

Attaches a gesture to the view with a higher precedence than gestures defined by the view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func highPriorityGesture(
    _ gesture: T,
    including mask: GestureMask = .all
) -> some View where T : Gesture
```

## Parameters 

`gesture`  

A gesture to attach to the view.

`mask`  

A value that controls how adding this gesture to the view affects other gestures recognized by the view and its subviews. Defaults to all.

## Discussion

Use this method when you need to define a high priority gesture to take precedence over the view’s existing gestures. The example below defines a custom gesture that prints a message to the console and attaches it to the view’s VStack. Inside the VStack a red heart Image defines its own TapGesture handler that also prints a message to the console, and a blue rectangle with no custom gesture handlers. Tapping or clicking any of the views results in a console message from the high priority gesture attached to the enclosing VStack.

```
struct HighPriorityGestureExample: View {
    @State private var message = "Message"
    let newGesture = TapGesture().onEnded {
        print("Tap on VStack.")
    }

    var body: some View {
        VStack(spacing:25) {
            Image(systemName: "heart.fill")
                .resizable()
                .frame(width: 75, height: 75)
                .padding()
                .foregroundColor(.red)
                .onTapGesture {
                    print("Tap on image.")
                }
            Rectangle()
                .fill(Color.blue)
        }
        .highPriorityGesture(newGesture)
        .frame(width: 200, height: 200)
        .border(Color.purple)
    }
}
```

## See Also

### Defining custom gestures

func highPriorityGesture&lt;T>(T, isEnabled: Bool) -> some View

Attaches a gesture to the view with a higher precedence than gestures defined by the view.

func highPriorityGesture&lt;T>(T, name: String, isEnabled: Bool) -> some View

Attaches a gesture to the view with a higher precedence than gestures defined by the view.

func handGestureShortcut(HandGestureShortcut, isEnabled: Bool) -> some View

Assigns a hand gesture shortcut to the modified control.

func defersSystemGestures(on: Edge.Set) -> some View

Sets the screen edge from which you want your gesture to take precedence over the system gesture.

protocol Gesture

An instance that matches a sequence of events to a gesture, and returns a stream of values for each of its states.

struct AnyGesture

A type-erased gesture.

struct HandActivationBehavior

An activation behavior specific to hand-driven input.

struct HandGestureShortcut

Hand gesture shortcuts describe finger and wrist movements that the user can perform in order to activate a button or toggle.

