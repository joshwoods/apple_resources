

- TabletopKit
-  EntityTableSeat 

Protocol

# EntityTableSeat

A protocol for seats at the table that you render using RealityKit.

TabletopKitRealityKitvisionOS 2.0+

``` source
protocol EntityTableSeat : TableSeat
```

## Overview

To render seats using an entity, follow these steps:

1.  Create a structure that conforms to this protocol.

2.  Set the State type alias to TableSeatState.

3.  Declare the `id` property as a TableSeatIdentifier structure.

4.  Declare the initialState property as a State structure.

5.  Implement an initializer that sets these properties and the entity property.

## Topics

### Rendering the equipment

var entity: Entity

The entity associated with the seat.

**Required**

## Relationships

### Inherits From

- Identifiable
- TableSeat

## See Also

### Seats

protocol TableSeat

A protocol for seats at the table that players occupy.

struct TableSeatIdentifier

A unique identifier for seats.

struct TableSeatState

The data associated with a seat that a player occupies.

protocol SeatState

A protocol for seat data that TabletopKit syncs between players.

