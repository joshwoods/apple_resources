

- RealityKit
- JointTransforms
-  reduce(\_:\_:) 

Instance Method

# reduce(\_:\_:)

Returns the result of combining the elements of the sequence using the given closure.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
func reduce(
    _ initialResult: Result,
    _ nextPartialResult: (Result, Self.Element) throws -> Result
) rethrows -> Result
```

## Parameters 

`initialResult`  

The value to use as the initial accumulating value. `initialResult` is passed to `nextPartialResult` the first time the closure is executed.

`nextPartialResult`  

A closure that combines an accumulating value and an element of the sequence into a new accumulating value, to be used in the next call of the `nextPartialResult` closure or returned to the caller.

## Return Value

The final accumulated value. If the sequence has no elements, the result is `initialResult`.

## Discussion

Use the `reduce(_:_:)` method to produce a single value from the elements of an entire sequence. For example, you can use this method on an array of numbers to find their sum or product.

The `nextPartialResult` closure is called sequentially with an accumulating value initialized to `initialResult` and each element of the sequence. This example shows how to find the sum of an array of numbers.

```
let numbers = [1, 2, 3, 4]
let numberSum = numbers.reduce(0, { x, y in
    x + y
})
// numberSum == 10
```

When `numbers.reduce(_:_:)` is called, the following steps occur:

1.  The `nextPartialResult` closure is called with `initialResult`—`0` in this case—and the first element of `numbers`, returning the sum: `1`.

2.  The closure is called again repeatedly with the previous call’s return value and each element of the sequence.

3.  When the sequence is exhausted, the last value returned from the closure is returned to the caller.

If the sequence has no elements, `nextPartialResult` is never executed and `initialResult` is the result of the call to `reduce(_:_:)`.

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

