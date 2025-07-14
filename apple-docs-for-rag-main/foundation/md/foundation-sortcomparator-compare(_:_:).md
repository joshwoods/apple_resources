

- Foundation
- SortComparator
-  compare(\_:\_:) 

Instance Method

# compare(\_:\_:)

Provides the relative ordering of two elements based on the sort order of the comparator.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func compare(
    _ lhs: Self.Compared,
    _ rhs: Self.Compared
) -> ComparisonResult
```

**Required**

## Parameters 

`lhs`  

The first element to compare.

`rhs`  

The second element to compare.

## Return Value

The relative ordering between the two elements according to the sort order of the comparator.

## See Also

### Using a Comparator

associatedtype Compared

A type that the sort comparator can compare.

**Required**

