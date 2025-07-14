

- SwiftUI
-  MagnifyGesture 

Structure

# MagnifyGesture

A gesture that recognizes a magnification motion and tracks the amount of magnification.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
struct MagnifyGesture
```

## Overview

A magnify gesture tracks how a magnification event sequence changes. To recognize a magnify gesture on a view, create and configure the gesture, and then add it to the view using the gesture(_:including:) modifier.

Add a magnify gesture to a Circle that changes its size while the user performs the gesture:

```
struct MagnifyGestureView: View {
    @GestureState private var magnifyBy = 1.0

    var magnification: some Gesture {
        MagnifyGesture()
            .updating($magnifyBy) { value, gestureState, transaction in
                gestureState = value.magnification
            }
    }

    var body: some View {
        Circle()
            .frame(width: 100, height: 100)
            .scaleEffect(magnifyBy)
            .gesture(magnification)
    }
}
```

## Topics

### Creating the gesture

init(minimumScaleDelta: CGFloat)

Creates a magnify gesture with a given minimum delta for the gesture to start.

var minimumScaleDelta: CGFloat

The minimum required delta before the gesture starts.

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

struct WindowDragGesture

A gesture that recognizes the motion of and handles dragging a window.

struct RotateGesture

A gesture that recognizes a rotation motion and tracks the angle of the rotation.

struct RotateGesture3D

A gesture that recognizes 3D rotation motion and tracks the angle and axis of the rotation.

struct GestureMask

Options that control how adding a gesture to a view affects other gestures recognized by the view and its subviews.

