

- TabletopKit
- TabletopGame
-  equipment(of:matching:) 

Instance Method

# equipment(of:matching:)

visionOS 2.0+

``` source
func equipment(
    of type: E.Type,
    matching id: EquipmentIdentifier
) -> E? where E : Equipment
```

## See Also

### Adding equipment to the game

var equipment: [any Equipment]

var equipmentIDs: [EquipmentIdentifier]

func equipment(matching: EquipmentIdentifier) -> (any Equipment)?

func equipment&lt;E>(of: E.Type) -> [E]

func equipment&lt;E>(of: E.Type, forEntity: Entity) -> E?

Retrieves the specified equipment type associated with an entity if it exists.

