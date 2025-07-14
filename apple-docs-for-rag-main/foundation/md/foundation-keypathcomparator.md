

- Foundation
-  KeyPathComparator 

Structure

# KeyPathComparator

A comparator that uses another sort comparator to provide the comparison of values at a key path.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct KeyPathComparator
```

## Topics

### Inspecting Key Path Comparators

let keyPath: any PartialKeyPath&lt;Compared> &amp; Sendable

The key path that the comparator uses to compare properties.

### Initializers

init&lt;Value, Comparator>(any KeyPath&lt;Compared, Value> &amp; Sendable, comparator: Comparator)

init&lt;Value, Comparator>(any KeyPath&lt;Compared, Value?> &amp; Sendable, comparator: Comparator)

init&lt;Value, Comparator>(any KeyPath&lt;Compared, Value> &amp; Sendable, comparator: Comparator, order: SortOrder)

init&lt;Value, Comparator>(any KeyPath&lt;Compared, Value?> &amp; Sendable, comparator: Comparator, order: SortOrder)

init&lt;Value>(any KeyPath&lt;Compared, Value> &amp; Sendable, order: SortOrder)

init&lt;Value>(any KeyPath&lt;Compared, Value?> &amp; Sendable, order: SortOrder)

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable
- SortComparator

## See Also

### Sorting

class NSSortDescriptor

An immutable description of how to order a collection of objects according to a property common to all the objects.

enum ComparisonResult

Constants that indicate sort order.

struct SortDescriptor

A serializable description of how to sort numerics and strings.

protocol SortComparator

A comparison algorithm for a specified type.

struct ComparableComparator

A comparator that compares types according to their conformance to the comparable protocol.

enum SortOrder

The orderings that you can perform sorts with.

