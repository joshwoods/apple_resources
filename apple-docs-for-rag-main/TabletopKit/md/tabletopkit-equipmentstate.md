

- TabletopKit
-  EquipmentState 

Protocol

# EquipmentState

A protocol for the equipment data that TabletopKit syncs between players.

visionOS 2.0+

``` source
protocol EquipmentState : Equatable
```

## Topics

### Getting the parent equipment

var parentID: EquipmentIdentifier

The identifier for the parent equipment that holds or contains this equipment.

**Required**

### Rendering the equipment

var boundingBox: Rect3D

A 3D bounding box that encloses the equipment.

**Required**

var pose: TableVisualState.Pose2D

The 2D position and rotation of the equipment relative to the equipment parent, or table.

**Required**

### Controlling the equipment

var lockedBy: PlayerIdentifier?

The identifier for the player who exclusively controls the equipment.

**Required**

var seatControl: ControllingSeats

The seats that can manipulate or interact with the equipment.

**Required**

## Relationships

### Inherits From

- Equatable

### Conforming Types

- BaseEquipmentState
- CardState
- DieState
- RawValueState

## See Also

### Equipment

protocol Equipment

A protocol for equipment that players directly interact with in a game.

protocol EntityEquipment

A protocol for equipment in a game that you render using RealityKit.

struct EquipmentIdentifier

A unique identifier for equipment.

struct BaseEquipmentState

A state for equipment that contains no equipment-specific data.

struct CardState

A state for cards that contains face up and down information.

struct DieState

A state for dice that contains the current value.

struct RawValueState

A state for equipment that contains a game-specific value.

enum ControllingSeats

The seats that can manipulate or interact with the equipment.

