

- TabletopKit
-  SetTurnAction 

Structure

# SetTurnAction

An action that sets the current seats participating in the current turn.

visionOS 2.0+

``` source
struct SetTurnAction
```

## Overview

To create a set turn action, use the setTurn(forSeat:context:) or a similar static method.

## Topics

### Getting the seats involved in a turn

var seatIDsInTurn: [TableSeatIdentifier]

The IDs of the seats that are part of the current turn.

### Instance Properties

var context: UInt64

An integer value that your game uses.

var playerID: Player.ID?

The ID of the player who is setting the turn.

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

struct UpdateCounterAction

An action that updates the game counter.

struct CreateBookmarkAction

An action that takes a snapshot of the game.

