

- SwiftUI
- View
-  gesture(\_:) 

Instance Method

# gesture(\_:)

Attaches a UIGestureRecognizerRepresentable to the view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
nonisolated
func gesture(_ representable: some UIGestureRecognizerRepresentable) -> some View
```

## Parameters 

`representable`  

The UIGestureRecognizerRepresentable that creates and manages a gesture recognizer.

## Return Value

A view with a UIGestureRecognizerRepresentable attached.

## See Also

### Recognizing gestures that change over time

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

struct RotateGesture

A gesture that recognizes a rotation motion and tracks the angle of the rotation.

struct RotateGesture3D

A gesture that recognizes 3D rotation motion and tracks the angle and axis of the rotation.

struct GestureMask

Options that control how adding a gesture to a view affects other gestures recognized by the view and its subviews.

