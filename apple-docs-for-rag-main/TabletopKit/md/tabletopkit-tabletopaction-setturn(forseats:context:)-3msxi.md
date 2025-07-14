

- TabletopKit
- TabletopAction
-  setTurn(forSeats:context:) 

Type Method

# setTurn(forSeats:context:)

visionOS 2.0+

``` source
static func setTurn(
    forSeats seats: some Sequence,
    context: UInt64 = 0
) -> Self
```

Available when `Self` is `SetTurnAction`.

## See Also

### Taking turns

static func setTurn(forSeat: some TableSeat, context: UInt64) -> Self

static func setTurn(forSeats: some Sequence&lt;any TableSeat>, context: UInt64) -> Self

static func setTurn(matching: TableSeatIdentifier, context: UInt64) -> Self

static func setTurn(matching: [TableSeatIdentifier], context: UInt64) -> Self

