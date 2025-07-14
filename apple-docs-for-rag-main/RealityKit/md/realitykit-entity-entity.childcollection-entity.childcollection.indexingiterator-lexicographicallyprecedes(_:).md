

- RealityKit
- Entity
- Entity.ChildCollection
- Entity.ChildCollection.IndexingIterator
-  lexicographicallyPrecedes(\_:) 

Instance Method

# lexicographicallyPrecedes(\_:)

Returns a Boolean value indicating whether the sequence precedes another sequence in a lexicographical (dictionary) ordering, using the less-than operator (`

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
func lexicographicallyPrecedes(_ other: OtherSequence) -> Bool where OtherSequence : Sequence, Self.Element == OtherSequence.Element
```

Available when `Element` conforms to `Comparable`.

## Parameters 

`other`  

A sequence to compare to this sequence.

## Return Value

`true` if this sequence precedes `other` in a dictionary ordering; otherwise, `false`.

## Discussion

This example uses the `lexicographicallyPrecedes` method to test which array of integers comes first in a lexicographical ordering.

```
let a = [1, 2, 2, 2]
let b = [1, 2, 3, 4]

print(a.lexicographicallyPrecedes(b))
// Prints "true"
print(b.lexicographicallyPrecedes(b))
// Prints "false"
```

Note

This method implements the mathematical notion of lexicographical ordering, which has no connection to Unicode. If you are sorting strings to present to the end user, use `String` APIs that perform localized comparison.

Complexity

O(*m*), where *m* is the lesser of the length of the sequence and the length of `other`.

## See Also

### Comparing collections

func elementsEqual&lt;OtherSequence>(OtherSequence) -> Bool

Returns a Boolean value indicating whether this sequence and another sequence contain the same elements in the same order.

func elementsEqual&lt;OtherSequence>(OtherSequence, by: (Self.Element, OtherSequence.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether this sequence and another sequence contain equivalent elements in the same order, using the given predicate as the equivalence test.

func starts&lt;PossiblePrefix>(with: PossiblePrefix) -> Bool

Returns a Boolean value indicating whether the initial elements of the sequence are the same as the elements in another sequence.

func starts&lt;PossiblePrefix>(with: PossiblePrefix, by: (Self.Element, PossiblePrefix.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether the initial elements of the sequence are equivalent to the elements in another sequence, using the given predicate as the equivalence test.

func lexicographicallyPrecedes&lt;OtherSequence>(OtherSequence, by: (Self.Element, Self.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether the sequence precedes another sequence in a lexicographical (dictionary) ordering, using the given predicate to compare elements.

