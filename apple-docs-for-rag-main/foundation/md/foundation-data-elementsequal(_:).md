

- Foundation
- Data
-  elementsEqual(\_:) 

Instance Method

# elementsEqual(\_:)

Returns a Boolean value indicating whether this sequence and another sequence contain the same elements in the same order.

FoundationSwiftiOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func elementsEqual(_ other: OtherSequence) -> Bool where OtherSequence : Sequence, Self.Element == OtherSequence.Element
```

Available when `Element` conforms to `Equatable`.

## Parameters 

`other`  

A sequence to compare to this sequence.

## Return Value

`true` if this sequence and `other` contain the same elements in the same order.

## Discussion

At least one of the sequences must be finite.

This example tests whether one countable range shares the same elements as another countable range and an array.

```
let a = 1...3
let b = 1...10

print(a.elementsEqual(b))
// Prints "false"
print(a.elementsEqual([1, 2, 3]))
// Prints "true"
```

Complexity

O(*m*), where *m* is the lesser of the length of the sequence and the length of `other`.

## See Also

### Comparing Data

static func == (Data, Data) -> Bool

Returns `true` if the two `Data` arguments are equal.

func starts&lt;PossiblePrefix>(with: PossiblePrefix) -> Bool

Returns a Boolean value indicating whether the initial elements of the sequence are the same as the elements in another sequence.

func lexicographicallyPrecedes&lt;OtherSequence>(OtherSequence) -> Bool

Returns a Boolean value indicating whether the sequence precedes another sequence in a lexicographical (dictionary) ordering, using the less-than operator (`

func lexicographicallyPrecedes&lt;OtherSequence>(OtherSequence, by: (Self.Element, Self.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether the sequence precedes another sequence in a lexicographical (dictionary) ordering, using the given predicate to compare elements.

