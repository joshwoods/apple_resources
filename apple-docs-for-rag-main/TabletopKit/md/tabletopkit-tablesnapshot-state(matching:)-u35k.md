

- TabletopKit
- TableSnapshot
-  state(matching:) 

Instance Method

# state(matching:)

visionOS 2.0+

``` source
func state(matching equipmentID: EquipmentIdentifier) -> (any EquipmentState)?
```

## See Also

### Getting information on equipment

func equipment&lt;E>(of: E.Type) -> [(E, E.State)]

func equipment&lt;E>(of: E.Type, childrenOf: some Equipment) -> [(E, E.State)]

func equipment&lt;E>(of: E.Type, childrenOf: EquipmentIdentifier) -> [(E, E.State)]

func equipment&lt;E>(of: E.Type, matching: some Sequence&lt;EquipmentIdentifier>) -> [(E, E.State)]

func equipment&lt;E>(of: E.Type, matching: EquipmentIdentifier) -> (E, E.State)?

func equipmentIDs() -> [EquipmentIdentifier]

func equipmentIDs(childrenOf: some Equipment) -> [EquipmentIdentifier]

func equipmentIDs(childrenOf: EquipmentIdentifier) -> [EquipmentIdentifier]

func entity(matching: EquipmentIdentifier) -> Entity?

