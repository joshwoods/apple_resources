

- Swift
- Sequence
-  dropLast(\_:) 

Instance Method

# dropLast(\_:)

Returns a sequence containing all but the given number of final elements.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func dropLast(_ k: Int = 1) -> [Self.Element]
```

## Return Value

A sequence leaving off the specified number of elements.

## Discussion

The sequence must be finite. If the number of elements to drop exceeds the number of elements in the sequence, the result is an empty sequence.

```
let numbers = [1, 2, 3, 4, 5]
print(numbers.dropLast(2))
// Prints "[1, 2, 3]"
print(numbers.dropLast(10))
// Prints "[]"
```

Complexity

O(*n*), where *n* is the length of the sequence.

## See Also

### Excluding Elements

func dropFirst(Int) -> DropFirstSequence&lt;Self>

Returns a sequence containing all but the given number of initial elements.

func drop(while: (Self.Element) throws -> Bool) rethrows -> DropWhileSequence&lt;Self>

Returns a sequence by skipping the initial, consecutive elements that satisfy the given predicate.

func filter((Self.Element) throws -> Bool) rethrows -> [Self.Element]

Returns an array containing, in order, the elements of the sequence that satisfy the given predicate.

