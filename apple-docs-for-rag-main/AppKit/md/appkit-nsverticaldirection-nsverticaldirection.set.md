

- AppKit
- NSVerticalDirection
-  NSVerticalDirection.Set 

Structure

# NSVerticalDirection.Set

An efficient set of vertical directions.

Mac Catalyst 18.0+macOS 15.0+

``` source
@frozen
struct Set
```

## Topics

### Initializers

init(NSVerticalDirection)

Creates a set of directions containing only the specified direction.

### Instance Methods

func contains(NSVerticalDirection) -> Bool

func insert(NSVerticalDirection) -> (inserted: Bool, memberAfterInsert: NSVerticalDirection)

func remove(NSVerticalDirection) -> NSVerticalDirection?

func update(with: NSVerticalDirection) -> NSVerticalDirection?

### Type Properties

static let all: NSVerticalDirection.Set

A set containing all vertical directions (up and down)

static let down: NSVerticalDirection.Set

A set containing only the down direction.

static let up: NSVerticalDirection.Set

A set containing only the up direction.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- ExpressibleByArrayLiteral
- Hashable
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

