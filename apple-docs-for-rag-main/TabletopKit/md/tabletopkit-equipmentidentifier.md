

- TabletopKit
-  EquipmentIdentifier 

Structure

# EquipmentIdentifier

A unique identifier for equipment.

visionOS 2.0+

``` source
struct EquipmentIdentifier
```

## Overview

The equipment identifier needs to be unique across all instances of the same tabletop game.

## Topics

### Creating equipment identifiers

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

### Equipment

protocol Equipment

A protocol for equipment that players directly interact with in a game.

protocol EntityEquipment

A protocol for equipment in a game that you render using RealityKit.

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

enum ControllingSeats

The seats that can manipulate or interact with the equipment.

