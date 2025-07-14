

- TabletopKit
- RawValueState
-  init(rawValue:parentID:seatControl:pose:boundingBox:) 

Initializer

# init(rawValue:parentID:seatControl:pose:boundingBox:)

Creates a state for equipment using the specified raw value, location, and player interactions.

visionOS 2.0+

``` source
init(
    rawValue: UInt64,
    parentID: EquipmentIdentifier,
    seatControl: ControllingSeats = .any,
    pose: TableVisualState.Pose2D = .identity,
    boundingBox: Rect3D
)
```

## See Also

### Creating a die state

init(rawValue: UInt64, parentID: EquipmentIdentifier, seatControl: ControllingSeats, pose: TableVisualState.Pose2D, entity: Entity)

