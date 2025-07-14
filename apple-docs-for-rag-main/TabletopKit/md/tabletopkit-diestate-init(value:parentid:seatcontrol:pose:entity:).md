

- TabletopKit
- DieState
-  init(value:parentID:seatControl:pose:entity:) 

Initializer

# init(value:parentID:seatControl:pose:entity:)

Creates a die state with the given die value, parent, controlling seats, pose, and associated entity providing the bounding box.

TabletopKitRealityKitvisionOS 2.0+

``` source
init(
    value: Int,
    parentID: EquipmentIdentifier,
    seatControl: ControllingSeats = .any,
    pose: TableVisualState.Pose2D = .identity,
    entity: Entity
)
```

## See Also

### Creating a die state

init(value: Int, parentID: EquipmentIdentifier, seatControl: ControllingSeats, pose: TableVisualState.Pose2D, boundingBox: Rect3D)

Creates the state of a die using the specified current value, location, and player interactions.

