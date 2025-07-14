

- TabletopKit
-  StateBookmarkIdentifier 

Structure

# StateBookmarkIdentifier

A unique identifier for bookmarks.

visionOS 2.0+

``` source
struct StateBookmarkIdentifier
```

## Overview

A bookmark identifier needs to be unique across all instances of the same tabletop game.

## Topics

### Creating bookmark identifiers

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

### Bookmarks

struct StateBookmark

A snapshot of the game state at a point in time.

