

- TabletopKit
- TabletopAction
-  moveEquipment(matching:childOf:order:pose:context:) 

Type Method

# moveEquipment(matching:childOf:order:pose:context:)

visionOS 2.0+

``` source
static func moveEquipment(
    matching equipmentID: EquipmentIdentifier,
    childOf parentID: EquipmentIdentifier,
    order: MoveEquipmentAction.Order? = nil,
    pose: TableVisualState.Pose2D? = nil,
    context: UInt64 = 0
) -> Self
```

Available when `Self` is `MoveEquipmentAction`.

## See Also

### Moving equipment

static func moveEquipment(some Equipment, childOf: any Equipment, order: MoveEquipmentAction.Order?, pose: TableVisualState.Pose2D?, context: UInt64) -> Self

