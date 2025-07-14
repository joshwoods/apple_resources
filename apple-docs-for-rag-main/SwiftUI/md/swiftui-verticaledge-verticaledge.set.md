

- SwiftUI
- VerticalEdge
-  VerticalEdge.Set 

Structure

# VerticalEdge.Set

An efficient set of vertical edges.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@frozen
struct Set
```

## Topics

### Getting edge sets

static let all: VerticalEdge.Set

A set containing the top and bottom vertical edges.

static let top: VerticalEdge.Set

A set containing only the top vertical edge.

static let bottom: VerticalEdge.Set

A set containing only the bottom vertical edge.

### Creating an edge set

init(VerticalEdge)

Creates a set of edges containing only the specified vertical edge.

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

