

- AppKit
- NSCursor
- NSCursor.FrameResizeDirection
-  NSCursor.FrameResizeDirection.Set 

Structure

# NSCursor.FrameResizeDirection.Set

An efficient set of frame resize directions.

Mac Catalyst 18.0+macOS 15.0+

``` source
struct Set
```

## Topics

### Initializers

init(NSCursor.FrameResizeDirection)

Creates a set of directions containing only the specified direction.

### Instance Methods

func contains(NSCursor.FrameResizeDirection) -> Bool

func insert(NSCursor.FrameResizeDirection) -> (inserted: Bool, memberAfterInsert: NSCursor.FrameResizeDirection)

func remove(NSCursor.FrameResizeDirection) -> NSCursor.FrameResizeDirection?

func update(with: NSCursor.FrameResizeDirection) -> NSCursor.FrameResizeDirection?

### Type Properties

static let all: NSCursor.FrameResizeDirection.Set

A set containing the inward and outward resizing directions.

static let inward: NSCursor.FrameResizeDirection.Set

A set containing only the inward resize direction.

static let outward: NSCursor.FrameResizeDirection.Set

A set containing only the outward resize direction.

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- Hashable
- OptionSet
- RawRepresentable
- SetAlgebra

