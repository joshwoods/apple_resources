

- TabletopKit
-  MoveEquipmentAction 

Structure

# MoveEquipmentAction

An action that moves a piece of equipment on the table or changes the grouping.

visionOS 2.0+

``` source
struct MoveEquipmentAction
```

## Overview

To create a move equipment action, use the moveEquipment(_:childOf:order:pose:context:) or the moveEquipment(matching:childOf:order:pose:context:) static method.

## Topics

### Getting the equipment in the action

var equipmentID: EquipmentIdentifier

The ID of the equipment being moved.

var parentID: EquipmentIdentifier

The equipment ID the moved equipment is being grouped under

var order: MoveEquipmentAction.Order?

The order in which the equipment should be inserted.

enum Order

The possible orders of equipment.

### Getting the position of the equipment

var pose: TableVisualState.Pose2D?

The position the equipment being moved to

### Getting game-specific information

var context: UInt64

An integer value that your game uses.

### Instance Properties

var playerID: Player.ID?

The ID of the player who is moving the equipment.

## Relationships

### Conforms To

- Equatable
- Sendable
- TabletopAction

## See Also

### Actions

protocol TabletopAction

A protocol for objects that describe an action in a tabletop game.

struct UpdateEquipmentAction

An action that updates properties of equipment on the table.

struct SetTurnAction

An action that sets the current seats participating in the current turn.

struct UpdateCounterAction

An action that updates the game counter.

struct CreateBookmarkAction

An action that takes a snapshot of the game.

