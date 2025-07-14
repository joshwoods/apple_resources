

- TabularData
- AnyColumnSlice
-  lexicographicallyPrecedes(\_:by:) 

Instance Method

# lexicographicallyPrecedes(\_:by:)

Returns a Boolean value indicating whether the sequence precedes another sequence in a lexicographical (dictionary) ordering, using the given predicate to compare elements.

TabularDataSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func lexicographicallyPrecedes(
    _ other: OtherSequence,
    by areInIncreasingOrder: (Self.Element, Self.Element) throws -> Bool
) rethrows -> Bool where OtherSequence : Sequence, Self.Element == OtherSequence.Element
```

## Parameters 

`other`  

A sequence to compare to this sequence.

`areInIncreasingOrder`  

A predicate that returns `true` if its first argument should be ordered before its second argument; otherwise, `false`.

## Return Value

`true` if this sequence precedes `other` in a dictionary ordering as ordered by `areInIncreasingOrder`; otherwise, `false`.

## Discussion

The predicate must be a *strict weak ordering* over the elements. That is, for any elements `a`, `b`, and `c`, the following conditions must hold:

- `areInIncreasingOrder(a, a)` is always `false`. (Irreflexivity)

- If `areInIncreasingOrder(a, b)` and `areInIncreasingOrder(b, c)` are both `true`, then `areInIncreasingOrder(a, c)` is also `true`. (Transitive comparability)

- Two elements are *incomparable* if neither is ordered before the other according to the predicate. If `a` and `b` are incomparable, and `b` and `c` are incomparable, then `a` and `c` are also incomparable. (Transitive incomparability)

Note

This method implements the mathematical notion of lexicographical ordering, which has no connection to Unicode. If you are sorting strings to present to the end user, use `String` APIs that perform localized comparison instead.

Complexity

O(*m*), where *m* is the lesser of the length of the sequence and the length of `other`.

## See Also

### Comparing with Another Sequence

func starts&lt;PossiblePrefix>(with: PossiblePrefix, by: (Self.Element, PossiblePrefix.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether the initial elements of the sequence are equivalent to the elements in another sequence, using the given predicate as the equivalence test.

func elementsEqual&lt;OtherSequence>(OtherSequence, by: (Self.Element, OtherSequence.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether this sequence and another sequence contain equivalent elements in the same order, using the given predicate as the equivalence test.

