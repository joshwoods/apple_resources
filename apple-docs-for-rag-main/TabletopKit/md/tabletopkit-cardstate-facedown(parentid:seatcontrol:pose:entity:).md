

- TabletopKit
- CardState
-  faceDown(parentID:seatControl:pose:entity:) 

Type Method

# faceDown(parentID:seatControl:pose:entity:)

TabletopKitRealityKitvisionOS 2.0+

``` source
static func faceDown(
    parentID: EquipmentIdentifier,
    seatControl: ControllingSeats = .any,
    pose: TableVisualState.Pose2D = .identity,
    entity: Entity
) -> CardState
```

## See Also

### Creating a card state

init(faceUp: Bool, parentID: EquipmentIdentifier, seatControl: ControllingSeats, pose: TableVisualState.Pose2D, boundingBox: Rect3D)

Creates the state of a card using its visibility, location, and player interactions.

init(faceUp: Bool, parentID: EquipmentIdentifier, seatControl: ControllingSeats, pose: TableVisualState.Pose2D, entity: Entity)

Creates a card state with the given faceUp value, parent, controlling seats, pose, and associated entity providing the bounding box.

static func faceDown(parentID: EquipmentIdentifier, seatControl: ControllingSeats, pose: TableVisualState.Pose2D, boundingBox: Rect3D) -> CardState

static func faceUp(parentID: EquipmentIdentifier, seatControl: ControllingSeats, pose: TableVisualState.Pose2D, boundingBox: Rect3D) -> CardState

static func faceUp(parentID: EquipmentIdentifier, seatControl: ControllingSeats, pose: TableVisualState.Pose2D, entity: Entity) -> CardState

