

- TabletopKit
-  RawValueState 

Structure

# RawValueState

A state for equipment that contains a game-specific value.

visionOS 2.0+

``` source
struct RawValueState
```

## Topics

### Creating a die state

init(rawValue: UInt64, parentID: EquipmentIdentifier, seatControl: ControllingSeats, pose: TableVisualState.Pose2D, boundingBox: Rect3D)

Creates a state for equipment using the specified raw value, location, and player interactions.

init(rawValue: UInt64, parentID: EquipmentIdentifier, seatControl: ControllingSeats, pose: TableVisualState.Pose2D, entity: Entity)

### Getting the die data

var rawValue: UInt64

The integer value for this piece of equipment.

### Getting the parent equipment

var parentID: EquipmentIdentifier

The identifier for the parent equipment that holds or contains this equipment.

### Rendering the equipment

var boundingBox: Rect3D

A 3D bounding box that encloses the equipment.

var pose: TableVisualState.Pose2D

The 2D position and rotation of the equipment relative to the equipment parent, or table.

### Controlling the equipment

var lockedBy: PlayerIdentifier?

The identifier for the player who exclusively controls the equipment.

var seatControl: ControllingSeats

The seats that can manipulate or interact with the equipment.

## Relationships

### Conforms To

- Equatable
- EquipmentState
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

enum ControllingSeats

The seats that can manipulate or interact with the equipment.

