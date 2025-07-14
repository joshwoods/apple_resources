

- TabletopKit
-  TableSeatState 

Structure

# TableSeatState

The data associated with a seat that a player occupies.

visionOS 2.0+

``` source
struct TableSeatState
```

## Topics

### Creating a seat state structure

init(pose: TableVisualState.Pose2D, context: UInt64)

Creates the state of a seat using the specified pose and optional, game-specific data.

### Setting the data that syncs

var playerID: Player.ID?

The identifier for the player who occupies the seat.

var pose: TableVisualState.Pose2D

The position and orientation of the seat around the table.

## Relationships

### Conforms To

- SeatState
- Sendable

## See Also

### Seats

protocol TableSeat

A protocol for seats at the table that players occupy.

protocol EntityTableSeat

A protocol for seats at the table that you render using RealityKit.

struct TableSeatIdentifier

A unique identifier for seats.

protocol SeatState

A protocol for seat data that TabletopKit syncs between players.

