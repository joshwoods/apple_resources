

- RealityKit
- Entity
- Entity.ChildCollection
- Entity.ChildCollection.IndexingIterator
-  split(separator:maxSplits:omittingEmptySubsequences:) 

Instance Method

# split(separator:maxSplits:omittingEmptySubsequences:)

Returns the longest possible subsequences of the sequence, in order, around elements equal to the given element.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
func split(
    separator: Self.Element,
    maxSplits: Int = Int.max,
    omittingEmptySubsequences: Bool = true
) -> [ArraySlice]
```

Available when `Element` conforms to `Equatable`.

## Parameters 

`separator`  

The element that should be split upon.

`maxSplits`  

The maximum number of times to split the sequence, or one less than the number of subsequences to return. If `maxSplits + 1` subsequences are returned, the last one is a suffix of the original sequence containing the remaining elements. `maxSplits` must be greater than or equal to zero. The default value is `Int.max`.

`omittingEmptySubsequences`  

If `false`, an empty subsequence is returned in the result for each consecutive pair of `separator` elements in the sequence and for each instance of `separator` at the start or end of the sequence. If `true`, only nonempty subsequences are returned. The default value is `true`.

## Return Value

An array of subsequences, split from this sequence’s elements.

## Discussion

The resulting array consists of at most `maxSplits + 1` subsequences. Elements that are used to split the sequence are not returned as part of any subsequence.

The following examples show the effects of the `maxSplits` and `omittingEmptySubsequences` parameters when splitting a string at each space character (” “). The first use of `split` returns each word that was originally separated by one or more spaces.

```
let line = "BLANCHE:   I don't want realism. I want magic!"
print(line.split(separator: " ")
          .map(String.init))
// Prints "["BLANCHE:", "I", "don\'t", "want", "realism.", "I", "want", "magic!"]"
```

The second example passes `1` for the `maxSplits` parameter, so the original string is split just once, into two new strings.

```
print(line.split(separator: " ", maxSplits: 1)
          .map(String.init))
// Prints "["BLANCHE:", "  I don\'t want realism. I want magic!"]"
```

The final example passes `false` for the `omittingEmptySubsequences` parameter, so the returned array contains empty strings where spaces were repeated.

```
print(line.split(separator: " ", omittingEmptySubsequences: false)
          .map(String.init))
// Prints "["BLANCHE:", "", "", "I", "don\'t", "want", "realism.", "I", "want", "magic!"]"
```

Complexity

O(*n*), where *n* is the length of the sequence.

## See Also

### Splitting and joining entities

func split(maxSplits: Int, omittingEmptySubsequences: Bool, whereSeparator: (Self.Element) throws -> Bool) rethrows -> [ArraySlice&lt;Self.Element>]

Returns the longest possible subsequences of the sequence, in order, that don’t contain elements satisfying the given predicate. Elements that are used to split the sequence are not returned as part of any subsequence.

func joined() -> FlattenSequence&lt;Self>

Returns the elements of this sequence of sequences, concatenated.

func joined&lt;Separator>(separator: Separator) -> JoinedSequence&lt;Self>

Returns the concatenated elements of this sequence of sequences, inserting the given separator between each element.

func joined(separator: String) -> String

Returns a new string by concatenating the elements of the sequence, adding the given separator between each element.

typealias SubSequence

