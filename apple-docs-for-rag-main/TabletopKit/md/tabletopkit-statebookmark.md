

- TabletopKit
-  StateBookmark 

Structure

# StateBookmark

A snapshot of the game state at a point in time.

visionOS 2.0+

``` source
struct StateBookmark
```

## Overview

Add bookmarks between turns so that you can jump to a prior turn and continue gameplay from there. When you jump to a bookmark, you reset the game state back to that point in time.

To add a bookmark, use the createBookmark(_:context:) or similar method. To jump to a bookmark, use the jumpToBookmark(_:) or similar method.

## Topics

### Initializing bookmarks

init(id: StateBookmark.ID)

## Relationships

### Conforms To

- Equatable
- Identifiable
- Sendable

## See Also

### Bookmarks

struct StateBookmarkIdentifier

A unique identifier for bookmarks.

