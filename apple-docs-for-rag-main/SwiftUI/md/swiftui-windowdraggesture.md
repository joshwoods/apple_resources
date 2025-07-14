

- SwiftUI
-  WindowDragGesture 

Structure

# WindowDragGesture

A gesture that recognizes the motion of and handles dragging a window.

macOS 15.0+

``` source
struct WindowDragGesture
```

## Overview

To recognize a window drag gesture on a view, create and configure the gesture, and then add it to the view using the gesture(_:isEnabled:) modifier. Consider also letting the gesture handle events that activate the containing window so that dragging the containing window works even when it’s inactive.

To add a window drag gesture to a Circle and change its color while a user performs the window drag gesture:

```
struct MyView: View {
    @GestureState var isDraggingWindow = false

    var dragWindow: some Gesture {
        WindowDragGesture()
            .updating($isDraggingWindow) { _, state, _ in
                state = true
            }
    }

    var body: some View {
        Circle()
            .fill(isDraggingWindow ? Color.green : .blue)
            .frame(width: 50, height: 50)
            .gesture(dragWindow)
            .allowsWindowActivationEvents()
    }
}
```

## Topics

### Structures

struct Value

The properties of a window drag gesture.

### Initializers

init()

Creates a window drag gesture.

## Relationships

### Conforms To

- Gesture

## See Also

### Recognizing gestures that change over time

func gesture(some UIGestureRecognizerRepresentable) -> some View

Attaches a UIGestureRecognizerRepresentable to the view.

func gesture&lt;T>(T, isEnabled: Bool) -> some View

Attaches a gesture to the view with a lower precedence than gestures defined by the view.

func gesture&lt;T>(T, name: String, isEnabled: Bool) -> some View

Attaches a gesture to the view with a lower precedence than gestures defined by the view.

func gesture&lt;T>(T, including: GestureMask) -> some View

Attaches a gesture to the view with a lower precedence than gestures defined by the view.

struct DragGesture

A dragging motion that invokes an action as the drag-event sequence changes.

struct MagnifyGesture

A gesture that recognizes a magnification motion and tracks the amount of magnification.

struct RotateGesture

A gesture that recognizes a rotation motion and tracks the angle of the rotation.

struct RotateGesture3D

A gesture that recognizes 3D rotation motion and tracks the angle and axis of the rotation.

struct GestureMask

Options that control how adding a gesture to a view affects other gestures recognized by the view and its subviews.

