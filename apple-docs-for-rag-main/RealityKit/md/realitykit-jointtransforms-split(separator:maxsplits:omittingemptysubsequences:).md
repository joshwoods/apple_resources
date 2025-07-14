

- RealityKit
- JointTransforms
-  split(separator:maxSplits:omittingEmptySubsequences:) 

Instance Method

# split(separator:maxSplits:omittingEmptySubsequences:)

Returns the longest possible subsequences of the collection, in order, around elements equal to the given element.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
func split(
    separator: Self.Element,
    maxSplits: Int = Int.max,
    omittingEmptySubsequences: Bool = true
) -> [Self.SubSequence]
```

Available when `Element` conforms to `Equatable`.

## Parameters 

`separator`  

The element that should be split upon.

`maxSplits`  

The maximum number of times to split the collection, or one less than the number of subsequences to return. If `maxSplits + 1` subsequences are returned, the last one is a suffix of the original collection containing the remaining elements. `maxSplits` must be greater than or equal to zero. The default value is `Int.max`.

`omittingEmptySubsequences`  

If `false`, an empty subsequence is returned in the result for each consecutive pair of `separator` elements in the collection and for each instance of `separator` at the start or end of the collection. If `true`, only nonempty subsequences are returned. The default value is `true`.

## Return Value

An array of subsequences, split from this collection’s elements.

## Discussion

The resulting array consists of at most `maxSplits + 1` subsequences. Elements that are used to split the collection are not returned as part of any subsequence.

The following examples show the effects of the `maxSplits` and `omittingEmptySubsequences` parameters when splitting a string at each space character (” “). The first use of `split` returns each word that was originally separated by one or more spaces.

```
let line = "BLANCHE:   I don't want realism. I want magic!"
print(line.split(separator: " "))
// Prints "["BLANCHE:", "I", "don\'t", "want", "realism.", "I", "want", "magic!"]"
```

The second example passes `1` for the `maxSplits` parameter, so the original string is split just once, into two new strings.

```
print(line.split(separator: " ", maxSplits: 1))
// Prints "["BLANCHE:", "  I don\'t want realism. I want magic!"]"
```

The final example passes `false` for the `omittingEmptySubsequences` parameter, so the returned array contains empty strings where spaces were repeated.

```
print(line.split(separator: " ", omittingEmptySubsequences: false))
// Prints "["BLANCHE:", "", "", "I", "don\'t", "want", "realism.", "I", "want", "magic!"]"
```

Complexity

O(*n*), where *n* is the length of the collection.

## See Also

### Accessing joint transforms

subscript(JointTransforms.Index) -> Transform

Accesses a single joint transform in the collection at the given index.

func allSatisfy((Self.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether every element of a sequence satisfies a given predicate.

func compactMap&lt;ElementOfResult>((Self.Element) throws -> ElementOfResult?) rethrows -> [ElementOfResult]

Returns an array containing the non-`nil` results of calling the given transformation with each element of this sequence.

func contains(Self.Element) -> Bool

Returns a Boolean value indicating whether the sequence contains the given element.

func contains(where: (Self.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether the sequence contains an element that satisfies the given predicate.

func difference&lt;C>(from: C) -> CollectionDifference&lt;Self.Element>

Returns the difference needed to produce this collection’s ordered elements from the given collection.

func difference&lt;C>(from: C, by: (C.Element, Self.Element) -> Bool) -> CollectionDifference&lt;Self.Element>

Returns the difference needed to produce this collection’s ordered elements from the given collection, using the given predicate as an equivalence test.

func distance(from: Self.Index, to: Self.Index) -> Int

func drop(while: (Self.Element) throws -> Bool) rethrows -> Self.SubSequence

Returns a subsequence by skipping elements while `predicate` returns `true` and returning the remaining elements.

func dropFirst(Int) -> Self.SubSequence

Returns a subsequence containing all but the given number of initial elements.

func dropLast(Int) -> Self.SubSequence

Returns a subsequence containing all but the specified number of final elements.

func elementsEqual&lt;OtherSequence>(OtherSequence) -> Bool

Returns a Boolean value indicating whether this sequence and another sequence contain the same elements in the same order.

func elementsEqual&lt;OtherSequence>(OtherSequence, by: (Self.Element, OtherSequence.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether this sequence and another sequence contain equivalent elements in the same order, using the given predicate as the equivalence test.

func enumerated() -> EnumeratedSequence&lt;Self>

Returns a sequence of pairs (*n*, *x*), where *n* represents a consecutive integer starting at zero and *x* represents an element of the sequence.

func filter((Self.Element) throws -> Bool) rethrows -> [Self.Element]

Returns an array containing, in order, the elements of the sequence that satisfy the given predicate.

