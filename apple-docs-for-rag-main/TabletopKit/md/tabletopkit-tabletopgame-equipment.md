

- TabletopKit
- TabletopGame
-  equipment 

Instance Property

# equipment

visionOS 2.0+

``` source
var equipment: [any Equipment] { get }
```

## See Also

### Adding equipment to the game

var equipmentIDs: [EquipmentIdentifier]

func equipment(matching: EquipmentIdentifier) -> (any Equipment)?

func equipment&lt;E>(of: E.Type) -> [E]

func equipment&lt;E>(of: E.Type, forEntity: Entity) -> E?

Retrieves the specified equipment type associated with an entity if it exists.

func equipment&lt;E>(of: E.Type, matching: EquipmentIdentifier) -> E?

