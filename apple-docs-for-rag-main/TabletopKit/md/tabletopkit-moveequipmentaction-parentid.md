

- TabletopKit
- MoveEquipmentAction
-  parentID 

Instance Property

# parentID

The equipment ID the moved equipment is being grouped under

visionOS 2.0+

``` source
var parentID: EquipmentIdentifier { get }
```

## See Also

### Getting the equipment in the action

var equipmentID: EquipmentIdentifier

The ID of the equipment being moved.

var order: MoveEquipmentAction.Order?

The order in which the equipment should be inserted.

enum Order

The possible orders of equipment.

