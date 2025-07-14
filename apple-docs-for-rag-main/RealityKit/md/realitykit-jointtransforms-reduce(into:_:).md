

- RealityKit
- JointTransforms
-  reduce(into:\_:) 

Instance Method

# reduce(into:\_:)

Returns the result of combining the elements of the sequence using the given closure.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
func reduce(
    into initialResult: Result,
    _ updateAccumulatingResult: (inout Result, Self.Element) throws -> ()
) rethrows -> Result
```

## Parameters 

`initialResult`  

The value to use as the initial accumulating value.

`updateAccumulatingResult`  

A closure that updates the accumulating value with an element of the sequence.

## Return Value

The final accumulated value. If the sequence has no elements, the result is `initialResult`.

## Discussion

Use the `reduce(into:_:)` method to produce a single value from the elements of an entire sequence. For example, you can use this method on an array of integers to filter adjacent equal entries or count frequencies.

This method is preferred over `reduce(_:_:)` for efficiency when the result is a copy-on-write type, for example an Array or a Dictionary.

The `updateAccumulatingResult` closure is called sequentially with a mutable accumulating value initialized to `initialResult` and each element of the sequence. This example shows how to build a dictionary of letter frequencies of a string.

```
let letters = "abracadabra"
let letterCount = letters.reduce(into: [:]) { counts, letter in
    counts[letter, default: 0] += 1
}
// letterCount == ["a": 5, "b": 2, "r": 2, "c": 1, "d": 1]
```

When `letters.reduce(into:_:)` is called, the following steps occur:

1.  The `updateAccumulatingResult` closure is called with the initial accumulating value—`[:]` in this case—and the first character of `letters`, modifying the accumulating value by setting `1` for the key `"a"`.

2.  The closure is called again repeatedly with the updated accumulating value and each element of the sequence.

3.  When the sequence is exhausted, the accumulating value is returned to the caller.

If the sequence has no elements, `updateAccumulatingResult` is never executed and `initialResult` is the result of the call to `reduce(into:_:)`.

Complexity

O(*n*), where *n* is the length of the sequence.

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

