

- TabletopKit
- TableSnapshot
-  state(for:) 

Instance Method

# state(for:)

visionOS 2.0+

``` source
func state(for equipment: E) -> E.State where E : Equipment
```

## See Also

### Getting information on seats

var turn: Set&lt;TableSeatIdentifier>

var seats: [any TableSeat]

var seatIDs: [TableSeatIdentifier]

func seat&lt;S>(of: S.Type, for: Player) -> (S, S.State)?

func seat&lt;S>(of: S.Type, matching: TableSeatIdentifier) -> (S, S.State)?

func seats&lt;S>(of: S.Type) -> [(S, S.State)]

func state(matching: TableSeatIdentifier) -> (any SeatState)?

func entity(forSeat: some EntityTableSeat) -> Entity?

func entity(matching: TableSeatIdentifier) -> Entity?

