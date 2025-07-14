

- Foundation
- Data
-  reversed() 

Instance Method

# reversed()

Returns a view presenting the elements of the collection in reverse order.

FoundationSwiftiOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func reversed() -> ReversedCollection
```

## Discussion

You can reverse a collection without allocating new space for its elements by calling this `reversed()` method. A `ReversedCollection` instance wraps an underlying collection and provides access to its elements in reverse order. This example prints the characters of a string in reverse order:

```
let word = "Backwards"
for char in word.reversed() {
    print(char, terminator: "")
}
// Prints "sdrawkcaB"
```

If you need a reversed collection of the same type, you may be able to use the collection’s sequence-based or collection-based initializer. For example, to get the reversed version of a string, reverse its characters and initialize a new `String` instance from the result.

```
let reversedWord = String(word.reversed())
print(reversedWord)
// Prints "sdrawkcaB"
```

Complexity

O(1)

## See Also

### Sorting Bytes

func sort(by: (Self.Element, Self.Element) throws -> Bool) rethrows

Sorts the collection in place, using the given predicate as the comparison between elements.

func sorted() -> [Self.Element]

Returns the elements of the sequence, sorted.

func sorted(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> [Self.Element]

Returns the elements of the sequence, sorted using the given predicate as the comparison between elements.

