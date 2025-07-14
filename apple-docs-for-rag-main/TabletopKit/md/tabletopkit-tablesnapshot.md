

- TabletopKit
-  TableSnapshot 

Structure

# TableSnapshot

A snapshot of the current state of the table.

visionOS 2.0+

``` source
struct TableSnapshot
```

## Topics

### Getting the table entity

var tableEntity: Entity?

### Getting information on seats

var turn: Set&lt;TableSeatIdentifier>

var seats: [any TableSeat]

var seatIDs: [TableSeatIdentifier]

func seat&lt;S>(of: S.Type, for: Player) -> (S, S.State)?

func seat&lt;S>(of: S.Type, matching: TableSeatIdentifier) -> (S, S.State)?

func seats&lt;S>(of: S.Type) -> [(S, S.State)]

func state&lt;E>(for: E) -> E.State

func state(matching: TableSeatIdentifier) -> (any SeatState)?

func entity(forSeat: some EntityTableSeat) -> Entity?

func entity(matching: TableSeatIdentifier) -> Entity?

### Getting cursors

var cursors: [TableCursor]

func cursor(matching: TableCursorIdentifier) -> TableCursor?

func cursors(forPlayer: Player) -> [TableCursor]

func cursors(hovering: EquipmentIdentifier) -> [TableCursor]

### Getting information on equipment

func equipment&lt;E>(of: E.Type) -> [(E, E.State)]

func equipment&lt;E>(of: E.Type, childrenOf: some Equipment) -> [(E, E.State)]

func equipment&lt;E>(of: E.Type, childrenOf: EquipmentIdentifier) -> [(E, E.State)]

func equipment&lt;E>(of: E.Type, matching: some Sequence&lt;EquipmentIdentifier>) -> [(E, E.State)]

func equipment&lt;E>(of: E.Type, matching: EquipmentIdentifier) -> (E, E.State)?

func equipmentIDs() -> [EquipmentIdentifier]

func equipmentIDs(childrenOf: some Equipment) -> [EquipmentIdentifier]

func equipmentIDs(childrenOf: EquipmentIdentifier) -> [EquipmentIdentifier]

func state(matching: EquipmentIdentifier) -> (any EquipmentState)?

func entity(matching: EquipmentIdentifier) -> Entity?

### Getting score counters

var counters: [ScoreCounter]

func counter(matching: ScoreCounter.ID) -> ScoreCounter?

### Instance Methods

func entity(forEquipment: some EntityEquipment) -> Entity?

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible

## See Also

### Interactions

class TabletopInteraction

A protocol for objects that manage the entire flow of players interacting with equipment.

struct TossableRepresentation

An object that represents geometric shapes that the player can throw during gameplay, such as dice.

struct TableVisualState

A structure that represents the appearance of an object on the table.

struct TableCursor

A visual indicator that represents the destination of player interactions with equipment.

struct TableCursorIdentifier

A unique identifier for cursors.

