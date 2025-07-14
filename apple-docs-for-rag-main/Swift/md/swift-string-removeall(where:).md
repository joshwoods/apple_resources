

- Swift
- String
-  removeAll(where:) 

Instance Method

# removeAll(where:)

Removes all the elements that satisfy the given predicate.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func removeAll(where shouldBeRemoved: (Self.Element) throws -> Bool) rethrows
```

## Parameters 

`shouldBeRemoved`  

A closure that takes an element of the sequence as its argument and returns a Boolean value indicating whether the element should be removed from the collection.

## Discussion

Use this method to remove every element in a collection that meets particular criteria. The order of the remaining elements is preserved. This example removes all the vowels from a string:

```
var phrase = "The rain in Spain stays mainly in the plain."

let vowels: Set = ["a", "e", "i", "o", "u"]
phrase.removeAll(where: { vowels.contains($0) })
// phrase == "Th rn n Spn stys mnly n th pln."
```

Complexity

O(*n*), where *n* is the length of the collection.

## See Also

### Removing Substrings

func remove(at: String.Index) -> Character

Removes and returns the character at the specified position.

func remove(at: Self.Index) -> Self.Element

Removes and returns the element at the specified position.

func removeAll(keepingCapacity: Bool)

Replaces this string with the empty string.

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

