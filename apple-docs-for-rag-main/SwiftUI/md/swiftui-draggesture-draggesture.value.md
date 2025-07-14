

- SwiftUI
- DragGesture
-  DragGesture.Value 

Structure

# DragGesture.Value

The attributes of a drag gesture.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
struct Value
```

## Topics

### Getting 2D position

var startLocation: CGPoint

The location of the drag gesture’s first event.

var location: CGPoint

The location of the drag gesture’s current event.

var predictedEndLocation: CGPoint

A prediction, based on the current drag velocity, of where the final location will be if dragging stopped now.

var translation: CGSize

The total translation from the start of the drag gesture to the current event of the drag gesture.

var predictedEndTranslation: CGSize

A prediction, based on the current drag velocity, of what the final translation will be if dragging stopped now.

### Getting 3D position

var startLocation3D: Point3D

The 3D start location of the drag gesture.

var location3D: Point3D

The 3D location of the drag gesture.

var predictedEndLocation3D: Point3D

A prediction of where the final location would be if dragging stopped now, based on the current drag velocity.

var translation3D: Vector3D

The translation of the drag gesture from `startLocation3D` to `location3D`.

var predictedEndTranslation3D: Vector3D

A prediction of what the final translation would be if dragging stopped now, based on the current drag velocity.

var startInputDevicePose3D: Pose3D?

The starting 3D pose of the device driving the drag, if one exists.

var inputDevicePose3D: Pose3D?

The 3D pose of the device driving the drag, if one exists.

### Handling changes over time

var time: Date

The time associated with the drag gesture’s current event.

var velocity: CGSize

The current drag velocity.

## Relationships

### Conforms To

- Equatable
- Sendable

