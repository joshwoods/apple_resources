

- TabularData
- DiscontiguousColumnSlice
-  sorted(using:) 

Instance Method

# sorted(using:)

Returns the elements of the sequence, sorted using the given comparator to compare elements.

TabularDataSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func sorted(using comparator: Comparator) -> [Self.Element] where Comparator : SortComparator, Self.Element == Comparator.Compared
```

## Parameters 

`comparator`  

The comparator to use in ordering elements

## Return Value

An array of the elements sorted using `comparator`.

