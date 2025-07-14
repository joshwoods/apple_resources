

- RealityKit
- Entity
- Entity.ChildCollection
- Entity.ChildCollection.IndexingIterator
-  sorted(using:) 

Instance Method

# sorted(using:)

Returns the elements of the sequence, sorted using the given array of `SortComparator`s to compare elements.

RealityKitSwiftiOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func sorted(using comparators: S) -> [Self.Element] where S : Sequence, Comparator : SortComparator, Comparator == S.Element, Self.Element == Comparator.Compared
```

## Parameters 

`comparators`  

An array of comparators used to compare elements. The first comparator specifies the primary comparator to be used in sorting the sequence’s elements. Any subsequent comparators are used to further refine the order of elements with equal values.

## Return Value

An array of the elements sorted using `comparators`.

