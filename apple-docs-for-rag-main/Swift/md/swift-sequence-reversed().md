

- Swift
- Sequence
-  reversed() 

Instance Method

# reversed()

Returns an array containing the elements of this sequence in reverse order.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func reversed() -> [Self.Element]
```

## Return Value

An array containing the elements of this sequence in reverse order.

## Discussion

The sequence must be finite.

Complexity

O(*n*), where *n* is the length of the sequence.

## See Also

### Sorting Elements

func sorted() -> [Self.Element]

Returns the elements of the sequence, sorted.

func sorted(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> [Self.Element]

Returns the elements of the sequence, sorted using the given predicate as the comparison between elements.

