

- Swift
- Sequence
-  joined(separator:) 

Instance Method

# joined(separator:)

Returns the concatenated elements of this sequence of sequences, inserting the given separator between each element.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func joined(separator: Separator) -> JoinedSequence where Separator : Sequence, Separator.Element == Self.Element.Element
```

Available when `Element` conforms to `Sequence`.

## Parameters 

`separator`  

A sequence to insert between each of this sequence’s elements.

## Return Value

The joined sequence of elements.

## Discussion

This example shows how an array of `[Int]` instances can be joined, using another `[Int]` instance as the separator:

```
let nestedNumbers = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
let joined = nestedNumbers.joined(separator: [-1, -2])
print(Array(joined))
// Prints "[1, 2, 3, -1, -2, 4, 5, 6, -1, -2, 7, 8, 9]"
```

## See Also

### Splitting and Joining Elements

func split(maxSplits: Int, omittingEmptySubsequences: Bool, whereSeparator: (Self.Element) throws -> Bool) rethrows -> [ArraySlice&lt;Self.Element>]

Returns the longest possible subsequences of the sequence, in order, that don’t contain elements satisfying the given predicate. Elements that are used to split the sequence are not returned as part of any subsequence.

func split(separator: Self.Element, maxSplits: Int, omittingEmptySubsequences: Bool) -> [ArraySlice&lt;Self.Element>]

Returns the longest possible subsequences of the sequence, in order, around elements equal to the given element.

func joined() -> FlattenSequence&lt;Self>

Returns the elements of this sequence of sequences, concatenated.

func joined(separator: String) -> String

Returns a new string by concatenating the elements of the sequence, adding the given separator between each element.

