

- SwiftUI
- SpatialEventCollection
- SpatialEventCollection.Event
-  targetedEntity 

Instance Property

# targetedEntity

The entity target for this touch, if one exists.

visionOS 1.0+

``` source
var targetedEntity: Entity?
```

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

struct InputDevicePose

A pose describing the input device like a hand controlling the event.

