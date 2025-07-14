

- Swift
- Sequence
-  reparentEquipment(\_:childrenOf:order:context:) 

Type Method

# reparentEquipment(\_:childrenOf:order:context:)

visionOS 2.0+

``` source
static func reparentEquipment(
    _ equipment: some Sequence,
    childrenOf parent: some Equipment,
    order: MoveEquipmentAction.Order? = nil,
    context: UInt64 = 0
) -> Self
```

Available when `Self` is `[MoveEquipmentAction]`.

