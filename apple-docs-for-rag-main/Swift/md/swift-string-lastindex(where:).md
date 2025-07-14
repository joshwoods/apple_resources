

- Swift
- String
-  lastIndex(where:) 

Instance Method

# lastIndex(where:)

Returns the index of the last element in the collection that matches the given predicate.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func lastIndex(where predicate: (Self.Element) throws -> Bool) rethrows -> Self.Index?
```

## Parameters 

`predicate`  

A closure that takes an element as its argument and returns a Boolean value that indicates whether the passed element represents a match.

## Return Value

The index of the last element in the collection that matches `predicate`, or `nil` if no elements match.

## Discussion

You can use the predicate to find an element of a type that doesn’t conform to the `Equatable` protocol or to find an element that matches particular criteria. This example finds the index of the last name that begins with the letter *A:*

```
let students = ["Kofi", "Abena", "Peter", "Kweku", "Akosua"]
if let i = students.lastIndex(where: { $0.hasPrefix("A") }) {
    print("\(students[i]) starts with 'A'!")
}
// Prints "Akosua starts with 'A'!"
```

Complexity

O(*n*), where *n* is the length of the collection.

## See Also

### Finding Characters

func contains(Self.Element) -> Bool

Returns a Boolean value indicating whether the sequence contains the given element.

func allSatisfy((Self.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether every element of a sequence satisfies a given predicate.

func contains(where: (Self.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether the sequence contains an element that satisfies the given predicate.

func first(where: (Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the first element of the sequence that satisfies the given predicate.

func firstIndex(of: Self.Element) -> Self.Index?

Returns the first index where the specified value appears in the collection.

func firstIndex(where: (Self.Element) throws -> Bool) rethrows -> Self.Index?

Returns the first index in which an element of the collection satisfies the given predicate.

func last(where: (Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the last element of the sequence that satisfies the given predicate.

func lastIndex(of: Self.Element) -> Self.Index?

Returns the last index where the specified value appears in the collection.

func max() -> Self.Element?

Returns the maximum element in the sequence.

func max&lt;T>(T, T) -> T

func max(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the maximum element in the sequence, using the given predicate as the comparison between elements.

func min() -> Self.Element?

Returns the minimum element in the sequence.

func min&lt;T>(T, T) -> T

func min(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the minimum element in the sequence, using the given predicate as the comparison between elements.

