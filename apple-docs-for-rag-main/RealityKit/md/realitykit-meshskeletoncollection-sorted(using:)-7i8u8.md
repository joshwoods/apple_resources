

- RealityKit
- MeshSkeletonCollection
-  sorted(using:) 

Instance Method

# sorted(using:)

Returns the elements of the sequence, sorted using the given comparator to compare elements.

RealityKitSwiftiOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func sorted(using comparator: Comparator) -> [Self.Element] where Comparator : SortComparator, Self.Element == Comparator.Compared
```

## Parameters 

`comparator`  

The comparator to use in ordering elements

## Return Value

An array of the elements sorted using `comparator`.

