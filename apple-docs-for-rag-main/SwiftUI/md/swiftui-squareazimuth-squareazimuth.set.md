

- SwiftUI
- SquareAzimuth
-  SquareAzimuth.Set 

Structure

# SquareAzimuth.Set

visionOS 2.0+

``` source
@frozen
struct Set
```

## Topics

### Initializers

init(SquareAzimuth)

Creates a set containing only the specified SquareAzimuth.

### Instance Methods

func contains(SquareAzimuth) -> Bool

Returns a Boolean value that indicates whether the set contains the specified SquareAzimuth.

### Type Properties

static let all: SquareAzimuth.Set

A set containing all four of the SquareAzimuth constants.

static let back: SquareAzimuth.Set

A set containing only SquareAzimuth.back.

static let front: SquareAzimuth.Set

A set containing only SquareAzimuth.front.

static let left: SquareAzimuth.Set

A set containing only SquareAzimuth.left.

static let right: SquareAzimuth.Set

A set containing only SquareAzimuth.right.

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

