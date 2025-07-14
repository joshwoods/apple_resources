

- RealityKit
- JointTransforms
-  partition(by:) 

Instance Method

# partition(by:)

Reorders the elements of the collection such that all the elements that match the given predicate are after all the elements that don’t match.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
mutating func partition(by belongsInSecondPartition: (Self.Element) throws -> Bool) rethrows -> Self.Index
```

## Parameters 

`belongsInSecondPartition`  

A predicate used to partition the collection. All elements satisfying this predicate are ordered after all elements not satisfying it.

## Return Value

The index of the first element in the reordered collection that matches `belongsInSecondPartition`. If no elements in the collection match `belongsInSecondPartition`, the returned index is equal to the collection’s `endIndex`.

## Discussion

After partitioning a collection, there is a pivot index `p` where no element before `p` satisfies the `belongsInSecondPartition` predicate and every element at or after `p` satisfies `belongsInSecondPartition`. This operation isn’t guaranteed to be stable, so the relative ordering of elements within the partitions might change.

In the following example, an array of numbers is partitioned by a predicate that matches elements greater than 30.

```
var numbers = [30, 40, 20, 30, 30, 60, 10]
let p = numbers.partition(by: { $0 > 30 })
// p == 5
// numbers == [30, 10, 20, 30, 30, 60, 40]
```

The `numbers` array is now arranged in two partitions. The first partition, `numbers[..

```
let first = numbers[..

Note that the order of elements in both partitions changed. That is, `40` appears before `60` in the original collection, but, after calling `partition(by:)`, `60` appears before `40`.

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

