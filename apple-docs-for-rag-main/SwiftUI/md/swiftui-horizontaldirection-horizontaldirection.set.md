

- SwiftUI
- HorizontalDirection
-  HorizontalDirection.Set 

Structure

# HorizontalDirection.Set

An efficient set of horizontal directions.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@frozen
struct Set
```

## Topics

### Initializers

init(HorizontalDirection)

Creates a set of directions containing only the specified direction.

### Type Properties

static let all: HorizontalDirection.Set

A set containing the leading and trailing horizontal directions.

static let leading: HorizontalDirection.Set

A set containing only the leading horizontal direction.

static let trailing: HorizontalDirection.Set

A set containing only the trailing horizontal direction.

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

