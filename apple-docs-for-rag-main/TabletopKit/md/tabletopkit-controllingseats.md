

- TabletopKit
-  ControllingSeats 

Enumeration

# ControllingSeats

The seats that can manipulate or interact with the equipment.

visionOS 2.0+

``` source
enum ControllingSeats
```

## Topics

### Seats

case any

Lets players in all seats interact with the equipment.

case restricted([TableSeatIdentifier])

Lets players in specific seats interact with the equipment.

case inherited

The value is inherited from the parent. The table implicit value is considered to be `.any`.

case current

Lets only seats currently in turn interact with the equipment.

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Equipment

protocol Equipment

A protocol for equipment that players directly interact with in a game.

protocol EntityEquipment

A protocol for equipment in a game that you render using RealityKit.

struct EquipmentIdentifier

A unique identifier for equipment.

protocol EquipmentState

A protocol for the equipment data that TabletopKit syncs between players.

struct BaseEquipmentState

A state for equipment that contains no equipment-specific data.

struct CardState

A state for cards that contains face up and down information.

struct DieState

A state for dice that contains the current value.

struct RawValueState

A state for equipment that contains a game-specific value.

