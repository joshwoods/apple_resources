

- RealityKit
- QueryResult
-  starts(with:by:) 

Instance Method

# starts(with:by:)

Returns a Boolean value indicating whether the initial elements of the sequence are equivalent to the elements in another sequence, using the given predicate as the equivalence test.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
func starts(
    with possiblePrefix: PossiblePrefix,
    by areEquivalent: (Self.Element, PossiblePrefix.Element) throws -> Bool
) rethrows -> Bool where PossiblePrefix : Sequence
```

## Parameters 

`possiblePrefix`  

A sequence to compare to this sequence.

`areEquivalent`  

A predicate that returns `true` if its two arguments are equivalent; otherwise, `false`.

## Return Value

`true` if the initial elements of the sequence are equivalent to the elements of `possiblePrefix`; otherwise, `false`. If `possiblePrefix` has no elements, the return value is `true`.

## Discussion

The predicate must be an *equivalence relation* over the elements. That is, for any elements `a`, `b`, and `c`, the following conditions must hold:

- `areEquivalent(a, a)` is always `true`. (Reflexivity)

- `areEquivalent(a, b)` implies `areEquivalent(b, a)`. (Symmetry)

- If `areEquivalent(a, b)` and `areEquivalent(b, c)` are both `true`, then `areEquivalent(a, c)` is also `true`. (Transitivity)

Complexity

O(*m*), where *m* is the lesser of the length of the sequence and the length of `possiblePrefix`.

## See Also

### Comparing sequences

func elementsEqual&lt;OtherSequence>(OtherSequence) -> Bool

Returns a Boolean value indicating whether this sequence and another sequence contain the same elements in the same order.

func elementsEqual&lt;OtherSequence>(OtherSequence, by: (Self.Element, OtherSequence.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether this sequence and another sequence contain equivalent elements in the same order, using the given predicate as the equivalence test.

func starts&lt;PossiblePrefix>(with: PossiblePrefix) -> Bool

Returns a Boolean value indicating whether the initial elements of the sequence are the same as the elements in another sequence.

