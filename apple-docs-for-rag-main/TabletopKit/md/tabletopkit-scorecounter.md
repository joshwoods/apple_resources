

- TabletopKit
-  ScoreCounter 

Structure

# ScoreCounter

An object that keeps a score in a tabletop game.

visionOS 2.0+

``` source
struct ScoreCounter
```

## Topics

### Creating score counters

init(id: ScoreCounter.ID, value: Int64)

Creates a score counter with a unique identifier and initial value.

### Getting score counter identifiers

var id: ScoreCounter.ID

A unique identifier for the score counter.

struct Identifier

A unique identifier for score counters.

### Getting score counter values

var value: Int64

The current value of the score counter.

## Relationships

### Conforms To

- Identifiable
- Sendable

