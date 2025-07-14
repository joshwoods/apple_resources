

- Foundation
- Data
-  removeLast(\_:) 

Instance Method

# removeLast(\_:)

Removes the given number of elements from the end of the collection.

FoundationSwiftiOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func removeLast(_ k: Int)
```

Available when `Self` is `Self.SubSequence`.

## Parameters 

`k`  

The number of elements to remove. `k` must be greater than or equal to zero, and must be less than or equal to the number of elements in the collection.

## Discussion

Complexity

O(1) if the collection conforms to `RandomAccessCollection`; otherwise, O(*k*), where *k* is the number of elements to remove.

