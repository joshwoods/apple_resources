

- TabletopKit
- TableSnapshot
-  equipmentIDs() 

Instance Method

# equipmentIDs()

visionOS 2.0+

``` source
func equipmentIDs() -> [EquipmentIdentifier]
```

## See Also

### Getting information on equipment

func equipment&lt;E>(of: E.Type) -> [(E, E.State)]

func equipment&lt;E>(of: E.Type, childrenOf: some Equipment) -> [(E, E.State)]

func equipment&lt;E>(of: E.Type, childrenOf: EquipmentIdentifier) -> [(E, E.State)]

func equipment&lt;E>(of: E.Type, matching: some Sequence&lt;EquipmentIdentifier>) -> [(E, E.State)]

func equipment&lt;E>(of: E.Type, matching: EquipmentIdentifier) -> (E, E.State)?

func equipmentIDs(childrenOf: some Equipment) -> [EquipmentIdentifier]

func equipmentIDs(childrenOf: EquipmentIdentifier) -> [EquipmentIdentifier]

func state(matching: EquipmentIdentifier) -> (any EquipmentState)?

func entity(matching: EquipmentIdentifier) -> Entity?

