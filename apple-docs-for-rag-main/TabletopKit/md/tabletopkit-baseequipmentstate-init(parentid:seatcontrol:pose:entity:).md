

- TabletopKit
- BaseEquipmentState
-  init(parentID:seatControl:pose:entity:) 

Initializer

# init(parentID:seatControl:pose:entity:)

TabletopKitRealityKitvisionOS 2.0+

``` source
init(
    parentID: EquipmentIdentifier,
    seatControl: ControllingSeats = .any,
    pose: TableVisualState.Pose2D = .identity,
    entity: Entity
)
```

## See Also

### Creating an equipment state

init(parentID: EquipmentIdentifier, seatControl: ControllingSeats, pose: TableVisualState.Pose2D, boundingBox: Rect3D)

Creates a base state for equipment using a parent, location, and player interactions.

