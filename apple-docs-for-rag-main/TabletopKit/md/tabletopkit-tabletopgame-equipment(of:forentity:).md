

- TabletopKit
- TabletopGame
-  equipment(of:forEntity:) 

Instance Method

# equipment(of:forEntity:)

Retrieves the specified equipment type associated with an entity if it exists.

TabletopKitRealityKitvisionOS 2.0+

``` source
func equipment(
    of type: E.Type,
    forEntity entity: Entity
) -> E? where E : EntityEquipment
```

## Parameters 

`type`  

The type of equipment to retrieve.

`entity`  

The entity that’s associated with the equipment type you want to find.

## Return Value

The equipment associated with the entity if it exists; otherwise, `nil`.

## Discussion

You can use this method to create custom interactions.

## See Also

### Adding equipment to the game

var equipment: [any Equipment]

var equipmentIDs: [EquipmentIdentifier]

func equipment(matching: EquipmentIdentifier) -> (any Equipment)?

func equipment&lt;E>(of: E.Type) -> [E]

func equipment&lt;E>(of: E.Type, matching: EquipmentIdentifier) -> E?

