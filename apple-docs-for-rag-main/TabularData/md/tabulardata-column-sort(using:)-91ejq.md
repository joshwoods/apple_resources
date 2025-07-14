

- TabularData
- Column
-  sort(using:) 

Instance Method

# sort(using:)

Sorts the collection using the given comparator to compare elements.

TabularDataSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func sort(using comparator: Comparator) where Comparator : SortComparator, Self.Element == Comparator.Compared
```

Available when `Self` conforms to `RandomAccessCollection`.

## Parameters 

`comparator`  

The sort comparator used to compare elements.

