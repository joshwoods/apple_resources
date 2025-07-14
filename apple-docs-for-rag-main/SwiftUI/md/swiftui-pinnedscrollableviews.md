

- SwiftUI
-  PinnedScrollableViews 

Structure

# PinnedScrollableViews

A set of view types that may be pinned to the bounds of a scroll view.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
struct PinnedScrollableViews
```

## Mentioned in 

Grouping data with lazy stack views

## Topics

### Getting scrollable view types

static let sectionHeaders: PinnedScrollableViews

The header view of each `Section` will be pinned.

static let sectionFooters: PinnedScrollableViews

The footer view of each `Section` will be pinned.

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Dynamically arranging views in one dimension

Grouping data with lazy stack views

Split content into logical sections inside lazy stack views.

Creating performant scrollable stacks

Display large numbers of repeated views efficiently with scroll views, stack views, and lazy stacks.

struct LazyHStack

A view that arranges its children in a line that grows horizontally, creating items only as needed.

struct LazyVStack

A view that arranges its children in a line that grows vertically, creating items only as needed.

