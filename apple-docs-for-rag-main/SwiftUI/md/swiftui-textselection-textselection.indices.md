

- SwiftUI
- TextSelection
-  TextSelection.Indices 

Enumeration

# TextSelection.Indices

The indicies of the current selection.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
enum Indices
```

## Topics

### Enumeration Cases

case multiSelection(RangeSet&lt;String.Index>)

The range-set of the selections.

case selection(Range&lt;String.Index>)

The range of the single selection. This may also an represent insertion points if `range.lowerBound == range.upperBound`.

## Relationships

### Conforms To

- Equatable
- Hashable

