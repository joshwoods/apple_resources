

- Foundation
- NSMutableOrderedSet
-  sortRange(\_:options:usingComparator:) 

Instance Method

# sortRange(\_:options:usingComparator:)

Sorts the specified range of the mutable ordered set using the specified options and the comparison method specified by a given comparator block.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func sortRange(
    _ range: NSRange,
    options opts: NSSortOptions = [],
    usingComparator cmptr: (Any, Any) -> ComparisonResult
)
```

## Parameters 

`range`  

The range to sort.

`opts`  

A bitmask that specifies the options for the sort (whether it should be performed concurrently and whether it should be performed stably).

`cmptr`  

A comparator block.

## See Also

### Sorting Entries

func sort(using: [NSSortDescriptor])

Sorts the receiving ordered set using a given array of sort descriptors.

func sort(comparator: (Any, Any) -> ComparisonResult)

Sorts the mutable ordered set using the comparison method specified by the comparator block.

func sort(options: NSSortOptions, usingComparator: (Any, Any) -> ComparisonResult)

Sorts the mutable ordered set using the specified options and the comparison method specified by a given comparator block.

