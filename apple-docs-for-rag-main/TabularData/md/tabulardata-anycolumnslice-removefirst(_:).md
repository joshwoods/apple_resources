

- TabularData
- AnyColumnSlice
-  removeFirst(\_:) 

Instance Method

# removeFirst(\_:)

Removes the specified number of elements from the beginning of the collection.

TabularDataSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func removeFirst(_ k: Int)
```

Available when `Self` is `Self.SubSequence`.

## Parameters 

`k`  

The number of elements to remove. `k` must be greater than or equal to zero, and must be less than or equal to the number of elements in the collection.

## Discussion

Complexity

O(1) if the collection conforms to `RandomAccessCollection`; otherwise, O(*k*), where *k* is the specified number of elements.

## See Also

### Removing Elements

func popFirst() -> Self.Element?

Removes and returns the first element of the collection.

func popLast() -> Self.Element?

Removes and returns the last element of the collection.

func removeFirst() -> Self.Element

Removes and returns the first element of the collection.

func removeLast() -> Self.Element

Removes and returns the last element of the collection.

func removeLast(Int)

Removes the given number of elements from the end of the collection.

