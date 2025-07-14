

- Swift
- Sequence
-  dropFirst(\_:) 

Instance Method

# dropFirst(\_:)

Returns a sequence containing all but the given number of initial elements.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func dropFirst(_ k: Int = 1) -> DropFirstSequence
```

## Parameters 

`k`  

The number of elements to drop from the beginning of the sequence. `k` must be greater than or equal to zero.

## Return Value

A sequence starting after the specified number of elements.

## Discussion

If the number of elements to drop exceeds the number of elements in the sequence, the result is an empty sequence.

```
let numbers = [1, 2, 3, 4, 5]
print(numbers.dropFirst(2))
// Prints "[3, 4, 5]"
print(numbers.dropFirst(10))
// Prints "[]"
```

Complexity

O(1), with O(*k*) deferred to each iteration of the result, where *k* is the number of elements to drop from the beginning of the sequence.

## See Also

### Excluding Elements

func dropLast(Int) -> [Self.Element]

Returns a sequence containing all but the given number of final elements.

func drop(while: (Self.Element) throws -> Bool) rethrows -> DropWhileSequence&lt;Self>

Returns a sequence by skipping the initial, consecutive elements that satisfy the given predicate.

func filter((Self.Element) throws -> Bool) rethrows -> [Self.Element]

Returns an array containing, in order, the elements of the sequence that satisfy the given predicate.

