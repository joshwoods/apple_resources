

- Swift
- Array
-  removeLast(\_:) 

Instance Method

# removeLast(\_:)

Removes the specified number of elements from the end of the collection.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func removeLast(_ k: Int)
```

Available when `Self` conforms to `BidirectionalCollection`.

## Parameters 

`k`  

The number of elements to remove from the collection. `k` must be greater than or equal to zero and must not exceed the number of elements in the collection.

## Discussion

Attempting to remove more elements than exist in the collection triggers a runtime error.

Calling this method may invalidate all saved indices of this collection. Do not rely on a previously stored index value after altering a collection with any operation that can change its length.

Complexity

O(*k*), where *k* is the specified number of elements.

## See Also

### Removing Elements

func remove(at: Int) -> Element

Removes and returns the element at the specified position.

func removeFirst() -> Self.Element

Removes and returns the first element of the collection.

func removeFirst(Int)

Removes the specified number of elements from the beginning of the collection.

func removeLast() -> Self.Element

Removes and returns the last element of the collection.

func removeSubrange(Range&lt;Self.Index>)

Removes the elements in the specified subrange from the collection.

func removeSubrange&lt;R>(R)

Removes the elements in the specified subrange from the collection.

func removeAll(where: (Self.Element) throws -> Bool) rethrows

Removes all the elements that satisfy the given predicate.

func removeAll(keepingCapacity: Bool)

Removes all elements from the array.

func popLast() -> Self.Element?

Removes and returns the last element of the collection.

