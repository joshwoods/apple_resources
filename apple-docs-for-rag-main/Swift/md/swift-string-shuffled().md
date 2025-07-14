

- Swift
- String
-  shuffled() 

Instance Method

# shuffled()

Returns the elements of the sequence, shuffled.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func shuffled() -> [Self.Element]
```

## Return Value

A shuffled array of this sequence’s elements.

## Discussion

For example, you can shuffle the numbers between `0` and `9` by calling the `shuffled()` method on that range:

```
let numbers = 0...9
let shuffledNumbers = numbers.shuffled()
// shuffledNumbers == [1, 7, 6, 2, 8, 9, 4, 3, 5, 0]
```

This method is equivalent to calling `shuffled(using:)`, passing in the system’s default random generator.

Complexity

O(*n*), where *n* is the length of the sequence.

## See Also

### Reordering a String’s Characters

func sorted() -> [Self.Element]

Returns the elements of the sequence, sorted.

func sorted(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> [Self.Element]

Returns the elements of the sequence, sorted using the given predicate as the comparison between elements.

func reversed() -> ReversedCollection&lt;Self>

Returns a view presenting the elements of the collection in reverse order.

func shuffled&lt;T>(using: inout T) -> [Self.Element]

Returns the elements of the sequence, shuffled using the given generator as a source for randomness.

