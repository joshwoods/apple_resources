

- Swift
- String
-  remove(at:) 

Instance Method

# remove(at:)

Removes and returns the character at the specified position.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@discardableResult
mutating func remove(at i: String.Index) -> Character
```

## Parameters 

`i`  

The position of the character to remove. `i` must be a valid index of the string that is not equal to the string’s end index.

## Return Value

The character that was removed.

## Discussion

All the elements following `i` are moved to close the gap. This example removes the hyphen from the middle of a string.

```
var nonempty = "non-empty"
if let i = nonempty.firstIndex(of: "-") {
    nonempty.remove(at: i)
}
print(nonempty)
// Prints "nonempty"
```

Calling this method invalidates any existing indices for use with this string.

## See Also

### Removing Substrings

func remove(at: Self.Index) -> Self.Element

Removes and returns the element at the specified position.

func removeAll(keepingCapacity: Bool)

Replaces this string with the empty string.

func removeAll(where: (Self.Element) throws -> Bool) rethrows

Removes all the elements that satisfy the given predicate.

func removeFirst() -> Self.Element

Removes and returns the first element of the collection.

func removeFirst(Int)

Removes the specified number of elements from the beginning of the collection.

func removeLast() -> Self.Element

Removes and returns the last element of the collection.

func removeLast(Int)

Removes the specified number of elements from the end of the collection.

func removeSubrange(Range&lt;String.Index>)

Removes the characters in the given range.

func removeSubrange(Range&lt;Self.Index>)

Removes the elements in the specified subrange from the collection.

func removeSubrange&lt;R>(R)

Removes the elements in the specified subrange from the collection.

func filter((Self.Element) throws -> Bool) rethrows -> Self

Returns a new collection of the same type containing, in order, the elements of the original collection that satisfy the given predicate.

func drop(while: (Self.Element) throws -> Bool) rethrows -> Self.SubSequence

Returns a subsequence by skipping elements while `predicate` returns `true` and returning the remaining elements.

func dropFirst(Int) -> Self.SubSequence

Returns a subsequence containing all but the given number of initial elements.

func dropLast(Int) -> Self.SubSequence

Returns a subsequence containing all but the specified number of final elements.

func popLast() -> Self.Element?

Removes and returns the last element of the collection.

