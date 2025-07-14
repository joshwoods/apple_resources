

- Foundation
- NSMutableOrderedSet
-  sort(comparator:) 

Instance Method

# sort(comparator:)

Sorts the mutable ordered set using the comparison method specified by the comparator block.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func sort(comparator cmptr: (Any, Any) -> ComparisonResult)
```

## Parameters 

`cmptr`  

A comparator block.

## See Also

### Sorting Entries

func sort(using: [NSSortDescriptor])

Sorts the receiving ordered set using a given array of sort descriptors.

func sort(options: NSSortOptions, usingComparator: (Any, Any) -> ComparisonResult)

Sorts the mutable ordered set using the specified options and the comparison method specified by a given comparator block.

func sortRange(NSRange, options: NSSortOptions, usingComparator: (Any, Any) -> ComparisonResult)

Sorts the specified range of the mutable ordered set using the specified options and the comparison method specified by a given comparator block.

