

- SwiftUI
-  RotateGesture3D 

Structure

# RotateGesture3D

A gesture that recognizes 3D rotation motion and tracks the angle and axis of the rotation.

visionOS 1.0+

``` source
struct RotateGesture3D
```

## Overview

You can constrain this gesture to recognize rotation about a specific 3D axis. For example, `RotateGesture3D(constrainedToAxis: .x)` creates a gesture that recognizes rotation only around the global X axis. The axis you provide will be normalized.

A rotation gesture tracks how a rotation event sequence changes. To recognize a rotation gesture on a view, create and configure the gesture, and then add it to the view using the gesture(_:including:) modifier.

## Topics

### Creating the gesture

init(constrainedToAxis: RotationAxis3D?, minimumAngleDelta: Angle)

Creates a rotation gesture with a minimum delta for the gesture to start and axis to constrain measurement of rotation.

var minimumAngleDelta: Angle

The minimum angle delta before the gesture becomes active.

var constrainedAxis: RotationAxis3D?

An axis around which the rotation is constrained.

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

struct RotateGesture

A gesture that recognizes a rotation motion and tracks the angle of the rotation.

struct GestureMask

Options that control how adding a gesture to a view affects other gestures recognized by the view and its subviews.

