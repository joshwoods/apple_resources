

- TabletopKit
- DieState
-  init(value:parentID:seatControl:pose:boundingBox:) 

Initializer

# init(value:parentID:seatControl:pose:boundingBox:)

Creates the state of a die using the specified current value, location, and player interactions.

visionOS 2.0+

``` source
init(
    value: Int,
    parentID: EquipmentIdentifier,
    seatControl: ControllingSeats = .any,
    pose: TableVisualState.Pose2D = .identity,
    boundingBox: Rect3D
)
```

## See Also

### Creating a die state

init(value: Int, parentID: EquipmentIdentifier, seatControl: ControllingSeats, pose: TableVisualState.Pose2D, entity: Entity)

Creates a die state with the given die value, parent, controlling seats, pose, and associated entity providing the bounding box.

