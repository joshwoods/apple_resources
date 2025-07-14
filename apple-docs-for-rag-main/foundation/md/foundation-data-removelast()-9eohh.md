

- Foundation
- Data
-  removeLast() 

Instance Method

# removeLast()

Removes and returns the last element of the collection.

FoundationSwiftiOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@discardableResult
mutating func removeLast() -> Self.Element
```

Available when `Self` is `Self.SubSequence`.

## Return Value

The last element of the collection.

## Discussion

The collection must not be empty. To remove the last element of a collection that might be empty, use the `popLast()` method instead.

Complexity

O(1)

