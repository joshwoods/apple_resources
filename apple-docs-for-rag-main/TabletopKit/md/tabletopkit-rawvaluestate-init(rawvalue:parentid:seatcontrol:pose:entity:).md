

- TabletopKit
- RawValueState
-  init(rawValue:parentID:seatControl:pose:entity:) 

Initializer

# init(rawValue:parentID:seatControl:pose:entity:)

TabletopKitRealityKitvisionOS 2.0+

``` source
init(
    rawValue: UInt64,
    parentID: EquipmentIdentifier,
    seatControl: ControllingSeats = .any,
    pose: TableVisualState.Pose2D = .identity,
    entity: Entity
)
```

## See Also

### Creating a die state

init(rawValue: UInt64, parentID: EquipmentIdentifier, seatControl: ControllingSeats, pose: TableVisualState.Pose2D, boundingBox: Rect3D)

Creates a state for equipment using the specified raw value, location, and player interactions.

