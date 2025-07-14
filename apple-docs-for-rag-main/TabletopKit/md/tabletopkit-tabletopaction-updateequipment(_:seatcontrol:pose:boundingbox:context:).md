

- TabletopKit
- TabletopAction
-  updateEquipment(\_:seatControl:pose:boundingBox:context:) 

Type Method

# updateEquipment(\_:seatControl:pose:boundingBox:context:)

visionOS 2.0+

``` source
static func updateEquipment(
    _ equipment: E,
    seatControl: ControllingSeats? = nil,
    pose: TableVisualState.Pose2D? = nil,
    boundingBox: Rect3D? = nil,
    context: UInt64 = 0
) -> Self where E : Equipment, E.State == BaseEquipmentState
```

Available when `Self` is `UpdateEquipmentAction`.

## See Also

### Changing equipment state properties

static func updateEquipment&lt;E>(E, faceUp: Bool?, seatControl: ControllingSeats?, pose: TableVisualState.Pose2D?, boundingBox: Rect3D?, context: UInt64) -> Self

static func updateEquipment&lt;E>(E, rawValue: UInt64?, seatControl: ControllingSeats?, pose: TableVisualState.Pose2D?, boundingBox: Rect3D?, context: UInt64) -> Self

static func updateEquipment&lt;E>(E, state: E.State, context: UInt64) -> Self

static func updateEquipment&lt;E>(E, state: E.State, context: UInt64) -> Self

static func updateEquipment&lt;E>(E, state: E.State, context: UInt64) -> Self

static func updateEquipment&lt;E>(E, state: E.State, context: UInt64) -> Self

static func updateEquipment&lt;E>(E, value: Int?, seatControl: ControllingSeats?, pose: TableVisualState.Pose2D?, boundingBox: Rect3D?, context: UInt64) -> Self

