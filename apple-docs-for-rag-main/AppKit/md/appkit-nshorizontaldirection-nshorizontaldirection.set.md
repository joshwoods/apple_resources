

- AppKit
- NSHorizontalDirection
-  NSHorizontalDirection.Set 

Structure

# NSHorizontalDirection.Set

An efficient set of horizontal directions.

Mac Catalyst 18.0+macOS 15.0+

``` source
@frozen
struct Set
```

## Topics

### Initializers

init(NSHorizontalDirection)

Creates a set of horizontal directions containing only the specified direction.

### Instance Methods

func contains(NSHorizontalDirection) -> Bool

func insert(NSHorizontalDirection) -> (inserted: Bool, memberAfterInsert: NSHorizontalDirection)

func remove(NSHorizontalDirection) -> NSHorizontalDirection?

func update(with: NSHorizontalDirection) -> NSHorizontalDirection?

### Type Properties

static let all: NSHorizontalDirection.Set

A set containing the all horizontal directions (left and right).

static let left: NSHorizontalDirection.Set

A set containing only the left direction.

static let right: NSHorizontalDirection.Set

A set containing only the right direction.

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

