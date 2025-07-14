

- TabletopKit
- TabletopGame
-  equipment(matching:) 

Instance Method

# equipment(matching:)

visionOS 2.0+

``` source
func equipment(matching id: EquipmentIdentifier) -> (any Equipment)?
```

## See Also

### Adding equipment to the game

var equipment: [any Equipment]

var equipmentIDs: [EquipmentIdentifier]

func equipment&lt;E>(of: E.Type) -> [E]

func equipment&lt;E>(of: E.Type, forEntity: Entity) -> E?

Retrieves the specified equipment type associated with an entity if it exists.

func equipment&lt;E>(of: E.Type, matching: EquipmentIdentifier) -> E?

