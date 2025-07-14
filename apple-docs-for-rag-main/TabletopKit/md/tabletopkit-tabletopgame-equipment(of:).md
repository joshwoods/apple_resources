

- TabletopKit
- TabletopGame
-  equipment(of:) 

Instance Method

# equipment(of:)

visionOS 2.0+

``` source
func equipment(of type: E.Type) -> [E] where E : Equipment
```

## See Also

### Adding equipment to the game

var equipment: [any Equipment]

var equipmentIDs: [EquipmentIdentifier]

func equipment(matching: EquipmentIdentifier) -> (any Equipment)?

func equipment&lt;E>(of: E.Type, forEntity: Entity) -> E?

Retrieves the specified equipment type associated with an entity if it exists.

func equipment&lt;E>(of: E.Type, matching: EquipmentIdentifier) -> E?

