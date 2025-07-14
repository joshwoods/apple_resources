

- TabletopKit
-  UpdateEquipmentAction 

Structure

# UpdateEquipmentAction

An action that updates properties of equipment on the table.

visionOS 2.0+

``` source
struct UpdateEquipmentAction where State : EquipmentState
```

## Overview

To create an update equipment action, use the updateEquipment(_:state:context:) or a similar static method.

## Topics

### Getting the equipment in the action

var equipmentID: EquipmentIdentifier

The ID of the equipment to update.

### Getting the state of the equipment

var newState: State?

The new state of the equipment.

### Instance Properties

var context: UInt64

An integer value that your game uses.

var playerID: Player.ID?

The player performing the action.

## Relationships

### Conforms To

- Equatable
- TabletopAction

## See Also

### Actions

protocol TabletopAction

A protocol for objects that describe an action in a tabletop game.

struct MoveEquipmentAction

An action that moves a piece of equipment on the table or changes the grouping.

struct SetTurnAction

An action that sets the current seats participating in the current turn.

struct UpdateCounterAction

An action that updates the game counter.

struct CreateBookmarkAction

An action that takes a snapshot of the game.

