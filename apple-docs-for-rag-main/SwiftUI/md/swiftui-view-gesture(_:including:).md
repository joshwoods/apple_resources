

- SwiftUI
- View
-  gesture(\_:including:) 

Instance Method

# gesture(\_:including:)

Attaches a gesture to the view with a lower precedence than gestures defined by the view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func gesture(
    _ gesture: T,
    including mask: GestureMask = .all
) -> some View where T : Gesture
```

## Parameters 

`gesture`  

A gesture to attach to the view.

`mask`  

A value that controls how adding this gesture to the view affects other gestures recognized by the view and its subviews. Defaults to all.

## Mentioned in 

Adding interactivity with gestures

## Discussion

Use this method when you need to attach a gesture to a view. The example below defines a custom gesture that prints a message to the console and attaches it to the view’s VStack. Inside the VStack a red heart Image defines its own TapGesture handler that also prints a message to the console, and blue rectangle with no custom gesture handlers. Tapping or clicking the image prints a message to the console from the tap gesture handler on the image, while tapping or clicking the rectangle inside the VStack prints a message in the console from the enclosing vertical stack gesture handler.

```
struct GestureExample: View {
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
        .gesture(newGesture)
        .frame(width: 200, height: 200)
        .border(Color.purple)
    }
}
```

## See Also

### Recognizing gestures that change over time

func gesture(some UIGestureRecognizerRepresentable) -> some View

Attaches a UIGestureRecognizerRepresentable to the view.

func gesture&lt;T>(T, isEnabled: Bool) -> some View

Attaches a gesture to the view with a lower precedence than gestures defined by the view.

func gesture&lt;T>(T, name: String, isEnabled: Bool) -> some View

Attaches a gesture to the view with a lower precedence than gestures defined by the view.

struct DragGesture

A dragging motion that invokes an action as the drag-event sequence changes.

struct WindowDragGesture

A gesture that recognizes the motion of and handles dragging a window.

struct MagnifyGesture

A gesture that recognizes a magnification motion and tracks the amount of magnification.

struct RotateGesture

A gesture that recognizes a rotation motion and tracks the angle of the rotation.

struct RotateGesture3D

A gesture that recognizes 3D rotation motion and tracks the angle and axis of the rotation.

struct GestureMask

Options that control how adding a gesture to a view affects other gestures recognized by the view and its subviews.

