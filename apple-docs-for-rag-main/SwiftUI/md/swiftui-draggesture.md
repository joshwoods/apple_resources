

- SwiftUI
-  DragGesture 

Structure

# DragGesture

A dragging motion that invokes an action as the drag-event sequence changes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @preconcurrency
struct DragGesture
```

## Mentioned in 

Composing SwiftUI gestures

## Overview

To recognize a drag gesture on a view, create and configure the gesture, and then add it to the view using the gesture(_:including:) modifier.

Add a drag gesture to a Circle and change its color while the user performs the drag gesture:

```
struct DragGestureView: View {
    @State private var isDragging = false

    var drag: some Gesture {
        DragGesture()
            .onChanged { _ in self.isDragging = true }
            .onEnded { _ in self.isDragging = false }
    }

    var body: some View {
        Circle()
            .fill(self.isDragging ? Color.red : Color.blue)
            .frame(width: 100, height: 100, alignment: .center)
            .gesture(drag)
    }
}
```

## Topics

### Creating a drag gesture

init(minimumDistance: CGFloat, coordinateSpace: some CoordinateSpaceProtocol)

Creates a dragging gesture with the minimum dragging distance before the gesture succeeds and the coordinate space of the gesture’s location.

var minimumDistance: CGFloat

The minimum dragging distance before the gesture succeeds.

var coordinateSpace: CoordinateSpace

The coordinate space in which to receive location values.

### Deprecated initializers

init(minimumDistance: CGFloat, coordinateSpace: CoordinateSpace)

Creates a dragging gesture with the minimum dragging distance before the gesture succeeds and the coordinate space of the gesture’s location.

Deprecated

### Structures

struct Value

The attributes of a drag gesture.

### Initializers

init(minimumDistance:coordinateSpace:)

Creates a dragging gesture with the minimum dragging distance before the gesture succeeds and the coordinate space of the gesture’s location.

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

