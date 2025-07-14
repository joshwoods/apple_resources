

- TabletopKit
- TableSnapshot
-  seat(of:matching:) 

Instance Method

# seat(of:matching:)

visionOS 2.0+

``` source
func seat(
    of type: S.Type,
    matching seatID: TableSeatIdentifier
) -> (S, S.State)? where S : TableSeat
```

## See Also

### Getting information on seats

var turn: Set&lt;TableSeatIdentifier>

var seats: [any TableSeat]

var seatIDs: [TableSeatIdentifier]

func seat&lt;S>(of: S.Type, for: Player) -> (S, S.State)?

func seats&lt;S>(of: S.Type) -> [(S, S.State)]

func state&lt;E>(for: E) -> E.State

func state(matching: TableSeatIdentifier) -> (any SeatState)?

func entity(forSeat: some EntityTableSeat) -> Entity?

func entity(matching: TableSeatIdentifier) -> Entity?

