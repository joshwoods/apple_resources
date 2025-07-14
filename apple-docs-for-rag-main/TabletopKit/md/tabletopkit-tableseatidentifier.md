

- TabletopKit
-  TableSeatIdentifier 

Structure

# TableSeatIdentifier

A unique identifier for seats.

visionOS 2.0+

``` source
struct TableSeatIdentifier
```

## Overview

The seat identifier needs to be unique across all instances of the same tabletop game.

## Topics

### Creating seat identifiers

init(Int)

### Getting identifier values

let rawValue: Int

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Seats

protocol TableSeat

A protocol for seats at the table that players occupy.

protocol EntityTableSeat

A protocol for seats at the table that you render using RealityKit.

struct TableSeatState

The data associated with a seat that a player occupies.

protocol SeatState

A protocol for seat data that TabletopKit syncs between players.

