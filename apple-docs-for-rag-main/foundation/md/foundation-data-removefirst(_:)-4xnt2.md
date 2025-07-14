

- Foundation
- Data
-  removeFirst(\_:) 

Instance Method

# removeFirst(\_:)

Removes the specified number of elements from the beginning of the collection.

FoundationSwiftiOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func removeFirst(_ k: Int)
```

Available when `Self` is `Self.SubSequence`.

## Parameters 

`k`  

The number of elements to remove from the collection. `k` must be greater than or equal to zero and must not exceed the number of elements in the collection.

## Discussion

Attempting to remove more elements than exist in the collection triggers a runtime error.

Calling this method may invalidate all saved indices of this collection. Do not rely on a previously stored index value after altering a collection with any operation that can change its length.

Complexity

O(1) if the collection conforms to `RandomAccessCollection`; otherwise, O(*k*), where *k* is the specified number of elements.

