

- TabletopKit
- MoveEquipmentAction
-  equipmentID 

Instance Property

# equipmentID

The ID of the equipment being moved.

visionOS 2.0+

``` source
var equipmentID: EquipmentIdentifier { get }
```

## See Also

### Getting the equipment in the action

var parentID: EquipmentIdentifier

The equipment ID the moved equipment is being grouped under

var order: MoveEquipmentAction.Order?

The order in which the equipment should be inserted.

enum Order

The possible orders of equipment.

