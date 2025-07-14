

- TabletopKit
- CardState
-  init(faceUp:parentID:seatControl:pose:entity:) 

Initializer

# init(faceUp:parentID:seatControl:pose:entity:)

Creates a card state with the given faceUp value, parent, controlling seats, pose, and associated entity providing the bounding box.

TabletopKitRealityKitvisionOS 2.0+

``` source
init(
    faceUp: Bool,
    parentID: EquipmentIdentifier,
    seatControl: ControllingSeats = .any,
    pose: TableVisualState.Pose2D = .identity,
    entity: Entity
)
```

## See Also

### Creating a card state

init(faceUp: Bool, parentID: EquipmentIdentifier, seatControl: ControllingSeats, pose: TableVisualState.Pose2D, boundingBox: Rect3D)

Creates the state of a card using its visibility, location, and player interactions.

static func faceDown(parentID: EquipmentIdentifier, seatControl: ControllingSeats, pose: TableVisualState.Pose2D, boundingBox: Rect3D) -> CardState

static func faceDown(parentID: EquipmentIdentifier, seatControl: ControllingSeats, pose: TableVisualState.Pose2D, entity: Entity) -> CardState

static func faceUp(parentID: EquipmentIdentifier, seatControl: ControllingSeats, pose: TableVisualState.Pose2D, boundingBox: Rect3D) -> CardState

static func faceUp(parentID: EquipmentIdentifier, seatControl: ControllingSeats, pose: TableVisualState.Pose2D, entity: Entity) -> CardState

