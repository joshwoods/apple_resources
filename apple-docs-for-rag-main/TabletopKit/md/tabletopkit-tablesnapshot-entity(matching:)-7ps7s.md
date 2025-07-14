

- TabletopKit
- TableSnapshot
-  entity(matching:) 

Instance Method

# entity(matching:)

TabletopKitRealityKitvisionOS 2.0+

``` source
func entity(matching seatID: TableSeatIdentifier) -> Entity?
```

## See Also

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

