

- TabularData
- AnyColumnSlice
-  sort(using:) 

Instance Method

# sort(using:)

Sorts the collection using the given array of `SortComparator`s to compare elements.

TabularDataSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func sort(using comparators: S) where S : Sequence, Comparator : SortComparator, Comparator == S.Element, Self.Element == Comparator.Compared
```

Available when `Self` conforms to `RandomAccessCollection`.

## Parameters 

`comparators`  

An array of comparators used to compare elements. The first comparator specifies the primary comparator to be used in sorting the sequence’s elements. Any subsequent comparators are used to further refine the order of elements with equal values.

