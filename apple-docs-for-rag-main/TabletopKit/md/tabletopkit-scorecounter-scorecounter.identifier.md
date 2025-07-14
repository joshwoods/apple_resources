

- TabletopKit
- ScoreCounter
-  ScoreCounter.Identifier 

Structure

# ScoreCounter.Identifier

A unique identifier for score counters.

visionOS 2.0+

``` source
struct Identifier
```

## Overview

A score counter identifier needs to be unique across all instances of the same tabletop game.

## Topics

### Creating score counter identifiers

init(Int)

### Instance Properties

let rawValue: Int

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Getting score counter identifiers

var id: ScoreCounter.ID

A unique identifier for the score counter.

