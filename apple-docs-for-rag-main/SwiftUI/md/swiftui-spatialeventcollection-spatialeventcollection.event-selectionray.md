

- SwiftUI
- SpatialEventCollection
- SpatialEventCollection.Event
-  selectionRay 

Instance Property

# selectionRay

The 3D ray used to target the touch.

visionOS 1.0+

``` source
var selectionRay: Ray3D?
```

## See Also

### Locating the event

var location: CGPoint

The 2D location of the event.

var location3D: Point3D

The 3D location of the touch.

var inputDevicePose: SpatialEventCollection.Event.InputDevicePose?

The 3D position and orientation of the device controlling the touch, if one exists.

struct InputDevicePose

A pose describing the input device like a hand controlling the event.

var targetedEntity: Entity?

The entity target for this touch, if one exists.

