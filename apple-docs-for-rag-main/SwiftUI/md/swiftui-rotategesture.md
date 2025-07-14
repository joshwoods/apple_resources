

- SwiftUI
-  RotateGesture 

Structure

# RotateGesture

A gesture that recognizes a rotation motion and tracks the angle of the rotation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
struct RotateGesture
```

## Overview

A rotate gesture tracks how a rotation event sequence changes. To recognize a rotate gesture on a view, create and configure the gesture, and then add it to the view using the gesture(_:including:) modifier.

Add a rotate gesture to a Rectangle and apply a rotation effect:

```
struct RotateGestureView: View {
    @State private var angle = Angle(degrees: 0.0)

    var rotation: some Gesture {
        RotateGesture()
            .onChanged { value in
                angle = value.rotation
            }
    }

    var body: some View {
        Rectangle()
            .frame(width: 200, height: 200, alignment: .center)
            .rotationEffect(angle)
            .gesture(rotation)
    }
}
```

## Topics

### Creating the gesture

init(minimumAngleDelta: Angle)

Creates a rotation gesture with a minimum delta for the gesture to start.

var minimumAngleDelta: Angle

The minimum delta required before the gesture succeeds.

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

struct MagnifyGesture

A gesture that recognizes a magnification motion and tracks the amount of magnification.

struct RotateGesture3D

A gesture that recognizes 3D rotation motion and tracks the angle and axis of the rotation.

struct GestureMask

Options that control how adding a gesture to a view affects other gestures recognized by the view and its subviews.

