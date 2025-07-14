

- SwiftUI
- VerticalDirection
-  VerticalDirection.Set 

Structure

# VerticalDirection.Set

An efficient set of vertical directions.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@frozen
struct Set
```

## Topics

### Initializers

init(VerticalDirection)

Creates a set of directions containing only the specified direction.

### Type Properties

static let all: VerticalDirection.Set

A set containing the upward and downward vertical directions.

static let down: VerticalDirection.Set

A set containing only the trailing horizontal direction.

static let up: VerticalDirection.Set

A set containing only the leading horizontal direction.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

