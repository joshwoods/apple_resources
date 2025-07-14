

- TabletopKit
- TableSnapshot
-  seatIDs 

Instance Property

# seatIDs

visionOS 2.0+

``` source
var seatIDs: [TableSeatIdentifier] { get }
```

## See Also

### Getting information on seats

var turn: Set&lt;TableSeatIdentifier>

var seats: [any TableSeat]

func seat&lt;S>(of: S.Type, for: Player) -> (S, S.State)?

func seat&lt;S>(of: S.Type, matching: TableSeatIdentifier) -> (S, S.State)?

func seats&lt;S>(of: S.Type) -> [(S, S.State)]

func state&lt;E>(for: E) -> E.State

func state(matching: TableSeatIdentifier) -> (any SeatState)?

func entity(forSeat: some EntityTableSeat) -> Entity?

func entity(matching: TableSeatIdentifier) -> Entity?

