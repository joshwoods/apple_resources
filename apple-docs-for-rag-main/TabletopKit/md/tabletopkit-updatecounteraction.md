

- TabletopKit
-  UpdateCounterAction 

Structure

# UpdateCounterAction

An action that updates the game counter.

visionOS 2.0+

``` source
struct UpdateCounterAction
```

## Overview

To create an update counter action, use the updateCounter(_:context:) or the updateCounter(matching:value:context:) static method.

## Topics

### Getting counter information

var counterID: ScoreCounter.Identifier

The ID of the counter to update.

var newValue: Int64

The new value to set for the counter.

### Getting game-specific information

var context: UInt64

An integer value that your game uses.

### Instance Properties

var playerID: Player.ID?

The ID of the player who is updating the counter.

## Relationships

### Conforms To

- Equatable
- Sendable
- TabletopAction

## See Also

### Actions

protocol TabletopAction

A protocol for objects that describe an action in a tabletop game.

struct MoveEquipmentAction

An action that moves a piece of equipment on the table or changes the grouping.

struct UpdateEquipmentAction

An action that updates properties of equipment on the table.

struct SetTurnAction

An action that sets the current seats participating in the current turn.

struct CreateBookmarkAction

An action that takes a snapshot of the game.

