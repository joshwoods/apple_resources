

- RealityKit
- LowLevelMesh
- LowLevelMesh.PartsCollection
-  sort(using:) 

Instance Method

# sort(using:)

Sorts the collection using the given comparator to compare elements.

RealityKitSwiftiOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
mutating func sort(using comparator: Comparator) where Comparator : SortComparator, Self.Element == Comparator.Compared
```

Available when `Self` conforms to `RandomAccessCollection`.

## Parameters 

`comparator`  

The sort comparator used to compare elements.

