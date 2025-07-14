

- SwiftUI
- FrameResizeDirection
-  FrameResizeDirection.Set 

Structure

# FrameResizeDirection.Set

An efficient set of frame resize directions.

macOS 15.0+

``` source
@frozen
struct Set
```

## Topics

### Initializers

init(FrameResizeDirection)

Creates a set of directions containing only the specified direction.

### Type Properties

static let all: FrameResizeDirection.Set

A set containing the inward and outward resizing directions.

static let inward: FrameResizeDirection.Set

A set containing only the inward resize direction.

static let outward: FrameResizeDirection.Set

A set containing only the outward resize direction.

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

