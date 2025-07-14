

- TabularData
- DataFrame
- DataFrame.Rows
-  sorted(using:) 

Instance Method

# sorted(using:)

Returns the elements of the sequence, sorted using the given array of `SortComparator`s to compare elements.

TabularDataSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func sorted(using comparators: S) -> [Self.Element] where S : Sequence, Comparator : SortComparator, Comparator == S.Element, Self.Element == Comparator.Compared
```

## Parameters 

`comparators`  

An array of comparators used to compare elements. The first comparator specifies the primary comparator to be used in sorting the sequence’s elements. Any subsequent comparators are used to further refine the order of elements with equal values.

## Return Value

An array of the elements sorted using `comparators`.

