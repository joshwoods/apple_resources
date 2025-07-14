

- TabletopKit
- TableSnapshot
-  equipment(of:) 

Instance Method

# equipment(of:)

visionOS 2.0+

``` source
func equipment(of type: E.Type) -> [(E, E.State)] where E : Equipment
```

## See Also

### Getting information on equipment

func equipment&lt;E>(of: E.Type, childrenOf: some Equipment) -> [(E, E.State)]

func equipment&lt;E>(of: E.Type, childrenOf: EquipmentIdentifier) -> [(E, E.State)]

func equipment&lt;E>(of: E.Type, matching: some Sequence&lt;EquipmentIdentifier>) -> [(E, E.State)]

func equipment&lt;E>(of: E.Type, matching: EquipmentIdentifier) -> (E, E.State)?

func equipmentIDs() -> [EquipmentIdentifier]

func equipmentIDs(childrenOf: some Equipment) -> [EquipmentIdentifier]

func equipmentIDs(childrenOf: EquipmentIdentifier) -> [EquipmentIdentifier]

func state(matching: EquipmentIdentifier) -> (any EquipmentState)?

func entity(matching: EquipmentIdentifier) -> Entity?

