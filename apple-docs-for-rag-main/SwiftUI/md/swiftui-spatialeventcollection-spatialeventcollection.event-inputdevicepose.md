

- SwiftUI
- SpatialEventCollection
- SpatialEventCollection.Event
-  inputDevicePose 

Instance Property

# inputDevicePose

The 3D position and orientation of the device controlling the touch, if one exists.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 1.0+

``` source
var inputDevicePose: SpatialEventCollection.Event.InputDevicePose? { get set }
```

## See Also

### Locating the event

var location: CGPoint

The 2D location of the event.

var location3D: Point3D

The 3D location of the touch.

var selectionRay: Ray3D?

The 3D ray used to target the touch.

struct InputDevicePose

A pose describing the input device like a hand controlling the event.

var targetedEntity: Entity?

The entity target for this touch, if one exists.

