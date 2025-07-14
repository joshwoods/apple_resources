

- Swift
- Sequence
-  reparentEquipment(matching:childrenOf:order:context:) 

Type Method

# reparentEquipment(matching:childrenOf:order:context:)

visionOS 2.0+

``` source
static func reparentEquipment(
    matching equipmentIDs: some Sequence,
    childrenOf parentID: EquipmentIdentifier,
    order: MoveEquipmentAction.Order? = nil,
    context: UInt64 = 0
) -> Self
```

Available when `Self` is `[MoveEquipmentAction]`.

