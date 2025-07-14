

- TabletopKit
-  SeatState 

Protocol

# SeatState

A protocol for seat data that TabletopKit syncs between players.

visionOS 2.0+

``` source
protocol SeatState
```

## Topics

### Setting the data that syncs

var context: UInt64

An integer value that your game uses.

**Required**

var playerID: PlayerIdentifier?

The identifier for the player that occupies the seat.

**Required**

var pose: TableVisualState.Pose2D

The position and orientation of the seat in table space.

**Required**

## Relationships

### Conforming Types

- TableSeatState

## See Also

### Seats

protocol TableSeat

A protocol for seats at the table that players occupy.

protocol EntityTableSeat

A protocol for seats at the table that you render using RealityKit.

struct TableSeatIdentifier

A unique identifier for seats.

struct TableSeatState

The data associated with a seat that a player occupies.

