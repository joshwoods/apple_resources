

- TabularData
- AnyColumnSlice
-  popLast() 

Instance Method

# popLast()

Removes and returns the last element of the collection.

TabularDataSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func popLast() -> Self.Element?
```

Available when `Self` is `Self.SubSequence`.

## Return Value

The last element of the collection if the collection has one or more elements; otherwise, `nil`.

## Discussion

You can use `popLast()` to remove the last element of a collection that might be empty. The `removeLast()` method must be used only on a nonempty collection.

Complexity

O(1)

## See Also

### Removing Elements

func popFirst() -> Self.Element?

Removes and returns the first element of the collection.

func removeFirst() -> Self.Element

Removes and returns the first element of the collection.

func removeFirst(Int)

Removes the specified number of elements from the beginning of the collection.

func removeLast() -> Self.Element

Removes and returns the last element of the collection.

func removeLast(Int)

Removes the given number of elements from the end of the collection.

