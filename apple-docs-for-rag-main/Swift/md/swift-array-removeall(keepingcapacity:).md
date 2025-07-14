

- Swift
- Array
-  removeAll(keepingCapacity:) 

Instance Method

# removeAll(keepingCapacity:)

Removes all elements from the array.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func removeAll(keepingCapacity keepCapacity: Bool = false)
```

## Parameters 

`keepCapacity`  

Pass `true` to keep the existing capacity of the array after removing its elements. The default value is `false`.

## Discussion

Complexity

O(*n*), where *n* is the length of the array.

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

func removeLast(Int)

Removes the specified number of elements from the end of the collection.

func removeSubrange(Range&lt;Self.Index>)

Removes the elements in the specified subrange from the collection.

func removeSubrange&lt;R>(R)

Removes the elements in the specified subrange from the collection.

func removeAll(where: (Self.Element) throws -> Bool) rethrows

Removes all the elements that satisfy the given predicate.

func popLast() -> Self.Element?

Removes and returns the last element of the collection.

