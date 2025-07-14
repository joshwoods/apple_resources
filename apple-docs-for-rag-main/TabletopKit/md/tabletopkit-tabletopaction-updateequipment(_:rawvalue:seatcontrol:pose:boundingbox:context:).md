

- TabletopKit
- TabletopAction
-  updateEquipment(\_:rawValue:seatControl:pose:boundingBox:context:) 

Type Method

# updateEquipment(\_:rawValue:seatControl:pose:boundingBox:context:)

visionOS 2.0+

``` source
static func updateEquipment(
    _ equipment: E,
    rawValue: UInt64? = nil,
    seatControl: ControllingSeats? = nil,
    pose: TableVisualState.Pose2D? = nil,
    boundingBox: Rect3D? = nil,
    context: UInt64 = 0
) -> Self where E : Equipment, E.State == RawValueState
```

Available when `Self` is `UpdateEquipmentAction`.

## See Also

### Changing equipment state properties

static func updateEquipment&lt;E>(E, faceUp: Bool?, seatControl: ControllingSeats?, pose: TableVisualState.Pose2D?, boundingBox: Rect3D?, context: UInt64) -> Self

static func updateEquipment&lt;E>(E, seatControl: ControllingSeats?, pose: TableVisualState.Pose2D?, boundingBox: Rect3D?, context: UInt64) -> Self

static func updateEquipment&lt;E>(E, state: E.State, context: UInt64) -> Self

static func updateEquipment&lt;E>(E, state: E.State, context: UInt64) -> Self

static func updateEquipment&lt;E>(E, state: E.State, context: UInt64) -> Self

static func updateEquipment&lt;E>(E, state: E.State, context: UInt64) -> Self

static func updateEquipment&lt;E>(E, value: Int?, seatControl: ControllingSeats?, pose: TableVisualState.Pose2D?, boundingBox: Rect3D?, context: UInt64) -> Self

