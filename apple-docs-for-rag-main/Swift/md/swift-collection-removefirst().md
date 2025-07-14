

- Swift
- Collection
-  removeFirst() 

Instance Method

# removeFirst()

Removes and returns the first element of the collection.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@discardableResult
mutating func removeFirst() -> Self.Element
```

Available when `Self` is `Self.SubSequence`.

## Return Value

The first element of the collection.

## Discussion

The collection must not be empty.

Complexity

O(1)

## See Also

### Selecting and Excluding Elements

func popFirst() -> Self.Element?

Removes and returns the first element of the collection.

func removeFirst(Int)

Removes the specified number of elements from the beginning of the collection.

