

- TabletopKit
-  TableCursorIdentifier 

Structure

# TableCursorIdentifier

A unique identifier for cursors.

visionOS 2.0+

``` source
struct TableCursorIdentifier
```

## Overview

A cursor identifier is unique across all instances of the same tabletop game.

## Topics

### Creating cursor identifiers

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

### Interactions

class TabletopInteraction

A protocol for objects that manage the entire flow of players interacting with equipment.

struct TossableRepresentation

An object that represents geometric shapes that the player can throw during gameplay, such as dice.

struct TableSnapshot

A snapshot of the current state of the table.

struct TableVisualState

A structure that represents the appearance of an object on the table.

struct TableCursor

A visual indicator that represents the destination of player interactions with equipment.

