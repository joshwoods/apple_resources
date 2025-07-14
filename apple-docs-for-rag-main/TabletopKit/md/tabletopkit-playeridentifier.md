

- TabletopKit
-  PlayerIdentifier 

Structure

# PlayerIdentifier

A unique identifier for players.

visionOS 2.0+

``` source
struct PlayerIdentifier
```

## Overview

A player identifier is unique across all instances of the same tabletop game.

## Topics

### Creating player identifiers

init(uuid: UUID)

Creates a player identifier.

### Getting identifier values

let uuid: UUID

A universally unique value to identify a player.

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Players

struct Player

A player in a tabletop game.

