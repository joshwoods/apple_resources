

- TabletopKit
- TabletopAction
-  moveEquipment(\_:childOf:order:pose:context:) 

Type Method

# moveEquipment(\_:childOf:order:pose:context:)

visionOS 2.0+

``` source
static func moveEquipment(
    _ equipment: some Equipment,
    childOf parent: any Equipment,
    order: MoveEquipmentAction.Order? = nil,
    pose: TableVisualState.Pose2D? = nil,
    context: UInt64 = 0
) -> Self
```

Available when `Self` is `MoveEquipmentAction`.

## See Also

### Moving equipment

static func moveEquipment(matching: EquipmentIdentifier, childOf: EquipmentIdentifier, order: MoveEquipmentAction.Order?, pose: TableVisualState.Pose2D?, context: UInt64) -> Self

