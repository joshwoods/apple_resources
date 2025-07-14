

- Foundation
- NSOrderedSet
-  sortedArray(options:usingComparator:) 

Instance Method

# sortedArray(options:usingComparator:)

Returns an array that lists the receiving ordered set’s elements in ascending order, as determined by the comparison method specified by a given `NSComparator` block.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func sortedArray(
    options opts: NSSortOptions = [],
    usingComparator cmptr: (Any, Any) -> ComparisonResult
) -> [Any]
```

## Parameters 

`opts`  

A bitmask that specifies the options for the sort (whether it should be performed concurrently and whether it should be performed stably).

`cmptr`  

A comparator block.

## Return Value

An array that lists the receiving ordered set’s elements in ascending order, as determined by the comparison method specified `cmptr`.

## See Also

### Creating a Sorted Array

func sortedArray(using: [NSSortDescriptor]) -> [Any]

Returns an array of the ordered set’s elements sorted as specified by a given array of sort descriptors.

func sortedArray(comparator: (Any, Any) -> ComparisonResult) -> [Any]

Returns an array that lists the receiving ordered set’s elements in ascending order, as determined by the comparison method specified by a given `NSComparator` block

