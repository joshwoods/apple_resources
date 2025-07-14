

- TabletopKit
-  CreateBookmarkAction 

Structure

# CreateBookmarkAction

An action that takes a snapshot of the game.

visionOS 2.0+

``` source
struct CreateBookmarkAction
```

## Overview

To create a bookmark action, use the createBookmark(_:context:) or the createBookmark(id:context:) static method.

## Topics

### Getting the bookmark

var bookmark: StateBookmark

### Getting game-specific information

var context: UInt64

An integer value that your game uses.

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

struct UpdateCounterAction

An action that updates the game counter.

