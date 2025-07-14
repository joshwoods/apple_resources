

- SwiftUI
- DragGesture
- DragGesture.Value
-  translation3D 

Instance Property

# translation3D

The translation of the drag gesture from `startLocation3D` to `location3D`.

visionOS 1.0+

``` source
var translation3D: Vector3D { get }
```

## See Also

### Getting 3D position

var startLocation3D: Point3D

The 3D start location of the drag gesture.

var location3D: Point3D

The 3D location of the drag gesture.

var predictedEndLocation3D: Point3D

A prediction of where the final location would be if dragging stopped now, based on the current drag velocity.

var predictedEndTranslation3D: Vector3D

A prediction of what the final translation would be if dragging stopped now, based on the current drag velocity.

var startInputDevicePose3D: Pose3D?

The starting 3D pose of the device driving the drag, if one exists.

var inputDevicePose3D: Pose3D?

The 3D pose of the device driving the drag, if one exists.

