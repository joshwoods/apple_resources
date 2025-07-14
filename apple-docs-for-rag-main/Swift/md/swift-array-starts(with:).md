

- Swift
- Array
-  starts(with:) 

Instance Method

# starts(with:)

Returns a Boolean value indicating whether the initial elements of the sequence are the same as the elements in another sequence.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func starts(with possiblePrefix: PossiblePrefix) -> Bool where PossiblePrefix : Sequence, Self.Element == PossiblePrefix.Element
```

Available when `Element` conforms to `Equatable`.

## Parameters 

`possiblePrefix`  

A sequence to compare to this sequence.

## Return Value

`true` if the initial elements of the sequence are the same as the elements of `possiblePrefix`; otherwise, `false`. If `possiblePrefix` has no elements, the return value is `true`.

## Discussion

This example tests whether one countable range begins with the elements of another countable range.

```
let a = 1...3
let b = 1...10

print(b.starts(with: a))
// Prints "true"
```

Passing a sequence with no elements or an empty collection as `possiblePrefix` always results in `true`.

```
print(b.starts(with: []))
// Prints "true"
```

Complexity

O(*m*), where *m* is the lesser of the length of the sequence and the length of `possiblePrefix`.

## See Also

### Comparing Arrays

static func == (Array&lt;Element>, Array&lt;Element>) -> Bool

Returns a Boolean value indicating whether two arrays contain the same elements in the same order.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func elementsEqual&lt;OtherSequence>(OtherSequence) -> Bool

Returns a Boolean value indicating whether this sequence and another sequence contain the same elements in the same order.

func elementsEqual&lt;OtherSequence>(OtherSequence, by: (Self.Element, OtherSequence.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether this sequence and another sequence contain equivalent elements in the same order, using the given predicate as the equivalence test.

func starts&lt;PossiblePrefix>(with: PossiblePrefix, by: (Self.Element, PossiblePrefix.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether the initial elements of the sequence are equivalent to the elements in another sequence, using the given predicate as the equivalence test.

func lexicographicallyPrecedes&lt;OtherSequence>(OtherSequence) -> Bool

Returns a Boolean value indicating whether the sequence precedes another sequence in a lexicographical (dictionary) ordering, using the less-than operator (`

func lexicographicallyPrecedes&lt;OtherSequence>(OtherSequence, by: (Self.Element, Self.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether the sequence precedes another sequence in a lexicographical (dictionary) ordering, using the given predicate to compare elements.

