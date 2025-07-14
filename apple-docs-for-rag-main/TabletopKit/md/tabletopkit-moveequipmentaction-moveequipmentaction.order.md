

- TabletopKit
- MoveEquipmentAction
-  MoveEquipmentAction.Order 

Enumeration

# MoveEquipmentAction.Order

The possible orders of equipment.

visionOS 2.0+

``` source
enum Order
```

## Topics

### Orders

case first

Inserts the equipment at the beginning of the list

case last

Inserts the equipment at the end of the list

case before(EquipmentIdentifier)

Inserts the equipment before the specified equipment identifier.

case after(EquipmentIdentifier)

Inserts the equipment after the specified equipment identifier.

case atIndex(Int)

Inserts the equipment at a specific location Note: the equipment is inserted at a undefined location if the index provided is not valid

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Getting the equipment in the action

var equipmentID: EquipmentIdentifier

The ID of the equipment being moved.

var parentID: EquipmentIdentifier

The equipment ID the moved equipment is being grouped under

var order: MoveEquipmentAction.Order?

The order in which the equipment should be inserted.

