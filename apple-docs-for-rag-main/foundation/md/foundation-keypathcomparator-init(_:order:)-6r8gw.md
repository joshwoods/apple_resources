

- Foundation
- KeyPathComparator
-  init(\_:order:) 

Initializer

# init(\_:order:)

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    _ keyPath: any KeyPath & Sendable,
    order: SortOrder = .forward
) where Value : Comparable
```

## See Also

### Initializers

init&lt;Value, Comparator>(any KeyPath&lt;Compared, Value> &amp; Sendable, comparator: Comparator)

init&lt;Value, Comparator>(any KeyPath&lt;Compared, Value?> &amp; Sendable, comparator: Comparator)

init&lt;Value, Comparator>(any KeyPath&lt;Compared, Value> &amp; Sendable, comparator: Comparator, order: SortOrder)

init&lt;Value, Comparator>(any KeyPath&lt;Compared, Value?> &amp; Sendable, comparator: Comparator, order: SortOrder)

init&lt;Value>(any KeyPath&lt;Compared, Value?> &amp; Sendable, order: SortOrder)

