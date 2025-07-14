

- RealityKit
- Entity
- Entity.ChildCollection
- Entity.ChildCollection.IndexingIterator
-  shuffled() 

Instance Method

# shuffled()

Returns the elements of the sequence, shuffled.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

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

### Reordering entities

func sorted() -> [Self.Element]

Returns the elements of the sequence, sorted.

func sorted(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> [Self.Element]

Returns the elements of the sequence, sorted using the given predicate as the comparison between elements.

func reversed() -> [Self.Element]

Returns an array containing the elements of this sequence in reverse order.

func shuffled&lt;T>(using: inout T) -> [Self.Element]

Returns the elements of the sequence, shuffled using the given generator as a source for randomness.

