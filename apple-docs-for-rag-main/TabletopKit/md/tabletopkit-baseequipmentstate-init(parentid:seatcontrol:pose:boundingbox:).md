

- TabletopKit
- BaseEquipmentState
-  init(parentID:seatControl:pose:boundingBox:) 

Initializer

# init(parentID:seatControl:pose:boundingBox:)

Creates a base state for equipment using a parent, location, and player interactions.

visionOS 2.0+

``` source
init(
    parentID: EquipmentIdentifier,
    seatControl: ControllingSeats = .any,
    pose: TableVisualState.Pose2D = .identity,
    boundingBox: Rect3D = .init()
)
```

## See Also

### Creating an equipment state

init(parentID: EquipmentIdentifier, seatControl: ControllingSeats, pose: TableVisualState.Pose2D, entity: Entity)

