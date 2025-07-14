

- RealityKit
- JointTransforms
-  prefix(upTo:) 

Instance Method

# prefix(upTo:)

Returns a subsequence from the start of the collection up to, but not including, the specified position.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
func prefix(upTo end: Self.Index) -> Self.SubSequence
```

## Parameters 

`end`  

The “past the end” index of the resulting subsequence. `end` must be a valid index of the collection.

## Return Value

A subsequence up to, but not including, the `end` position.

## Discussion

The resulting subsequence *does not include* the element at the position `end`. The following example searches for the index of the number `40` in an array of integers, and then prints the prefix of the array up to, but not including, that index:

```
let numbers = [10, 20, 30, 40, 50, 60]
if let i = numbers.firstIndex(of: 40) {
    print(numbers.prefix(upTo: i))
}
// Prints "[10, 20, 30]"
```

Passing the collection’s starting index as the `end` parameter results in an empty subsequence.

```
print(numbers.prefix(upTo: numbers.startIndex))
// Prints "[]"
```

Using the `prefix(upTo:)` method is equivalent to using a partial half-open range as the collection’s subscript. The subscript notation is preferred over `prefix(upTo:)`.

```
if let i = numbers.firstIndex(of: 40) {
    print(numbers[..

Complexity

O(1)

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

