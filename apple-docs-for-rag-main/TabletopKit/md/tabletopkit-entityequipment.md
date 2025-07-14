

- TabletopKit
-  EntityEquipment 

Protocol

# EntityEquipment

A protocol for equipment in a game that you render using RealityKit.

TabletopKitRealityKitvisionOS 2.0+

``` source
protocol EntityEquipment : Equipment
```

## Overview

To render equipment using an entity, follow these steps:

1.  Create a structure that conforms to this protocol.

2.  Depending on the type of equipment, set the State type alias to either BaseEquipmentState, DieState, or CardState.

3.  Declare the `id` property as a EquipmentIdentifier structure.

4.  Declare the initialState property as a State structure.

5.  Implement an initializer that sets these properties and the entity property.

```
```

Optionally, implement the layoutChildren(for:visualState:) method for equipment that represents groups, and the restingOrientation(state:) method to provide a custom resting position. For example, implement the restingOrientation(state:) method to flip a card face down in a card game:

```
```

## Topics

### Displaying the equipment

var entity: Entity

The entity associated with the equipment.

**Required**

## Relationships

### Inherits From

- Equipment
- Identifiable

## See Also

### Equipment

protocol Equipment

A protocol for equipment that players directly interact with in a game.

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

enum ControllingSeats

The seats that can manipulate or interact with the equipment.

