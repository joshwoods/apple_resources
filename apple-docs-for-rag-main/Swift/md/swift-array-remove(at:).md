

- Swift
- Array
-  remove(at:) 

Instance Method

# remove(at:)

Removes and returns the element at the specified position.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@discardableResult
mutating func remove(at index: Int) -> Element
```

## Parameters 

`index`  

The position of the element to remove. `index` must be a valid index of the array.

## Return Value

The element at the specified index.

## Discussion

All the elements following the specified position are moved up to close the gap.

```
var measurements: [Double] = [1.1, 1.5, 2.9, 1.2, 1.5, 1.3, 1.2]
let removed = measurements.remove(at: 2)
print(measurements)
// Prints "[1.1, 1.5, 1.2, 1.5, 1.3, 1.2]"
```

Complexity

O(*n*), where *n* is the length of the array.

## See Also

### Removing Elements

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

func removeAll(keepingCapacity: Bool)

Removes all elements from the array.

func popLast() -> Self.Element?

Removes and returns the last element of the collection.

