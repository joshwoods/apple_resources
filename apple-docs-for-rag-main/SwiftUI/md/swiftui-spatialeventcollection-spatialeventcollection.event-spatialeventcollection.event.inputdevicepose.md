

- SwiftUI
- SpatialEventCollection
- SpatialEventCollection.Event
-  SpatialEventCollection.Event.InputDevicePose 

Structure

# SpatialEventCollection.Event.InputDevicePose

A pose describing the input device like a hand controlling the event.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+watchOS 11.0+

``` source
struct InputDevicePose
```

## Topics

### Getting the event type

var altitude: Angle

The altitude angle.

var azimuth: Angle

The azimuth angle.

var pose3D: Pose3D

The 3D pose of the input device.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Locating the event

var location: CGPoint

The 2D location of the event.

var location3D: Point3D

The 3D location of the touch.

var selectionRay: Ray3D?

The 3D ray used to target the touch.

var inputDevicePose: SpatialEventCollection.Event.InputDevicePose?

The 3D position and orientation of the device controlling the touch, if one exists.

var targetedEntity: Entity?

The entity target for this touch, if one exists.

