

- TabletopKit
- TableSnapshot
-  seat(of:for:) 

Instance Method

# seat(of:for:)

visionOS 2.0+

``` source
func seat(
    of type: S.Type,
    for player: Player
) -> (S, S.State)? where S : TableSeat
```

## See Also

### Getting information on seats

var turn: Set&lt;TableSeatIdentifier>

var seats: [any TableSeat]

var seatIDs: [TableSeatIdentifier]

func seat&lt;S>(of: S.Type, matching: TableSeatIdentifier) -> (S, S.State)?

func seats&lt;S>(of: S.Type) -> [(S, S.State)]

func state&lt;E>(for: E) -> E.State

func state(matching: TableSeatIdentifier) -> (any SeatState)?

func entity(forSeat: some EntityTableSeat) -> Entity?

func entity(matching: TableSeatIdentifier) -> Entity?

