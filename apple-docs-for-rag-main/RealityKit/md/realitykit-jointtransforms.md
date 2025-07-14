

- RealityKit
-  JointTransforms 

Structure

# JointTransforms

A set of animatable transform values for joints that collectively represent a single skeletal pose.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct JointTransforms
```

## Overview

This structure provides a template that informs an animation on how to animate a character. The resulting movement bases on the *from* (fromValue) , *to* (toValue) , or *by* values (byValue) you supply for a FromToByAnimation. The animation determines which joints take on the movement through its jointNames property.

## Animate an Entity’s Skeleton

The following code moves the joints of a 3D asset by specifying the joint, `joint1`, beginning, and ending values.

```
// Define the joint's pose at the start of the animation.
let fromTransforms: [Transform] = [Transform(scale: SIMD3(1, 2, 3), rotation: simd_quatf(ix: 5.0, iy: 6.0, iz: 7.0, r: 8.0), translation: SIMD3(10, 20, 30))]
let fromPose = JointTransforms(fromTransforms)

// Define the joint's pose at the end of the animation.
let toTransforms: [Transform] = [Transform(scale: SIMD3(10, 20, 30), rotation:
simd_quatf(ix: 50.0, iy: 60.0, iz: 70.0, r: 80.0), translation:
SIMD3(100, 200, 300)) ]
let toPose = JointTransforms(toTransforms)

// Indicate that the animation applies to the joint named 'joint1'.
let jointNames = ["joint1"]

// Configure the animation specifics.
var fromToBy = FromToByAnimation()
fromToBy.name = "anim"
fromToBy.blendLayer = 100
fromToBy.duration = 10.0
fromToBy.fillMode = .forwards
fromToBy.jointNames = jointNames
fromToBy.fromValue = fromPose
fromToBy.toValue = toPose
fromToBy.bindTarget = .transform

// Generate a resource from the animation.
let animationResource = fromToBy.create()
```

To run the animation on an entity and animate the joints, call `playAnimation(_:transitionDuration:startsPaused:)`. Optionally, you can control the animation’s playback by storing the returned controller object.

```
// Play the animation on an entity.
let entity = AnchorEntity(...)
let controller = entity.playAnimation(animationResource)

// Optionally control playback using the returned controller.
controller.pause()
```

## Topics

### Creating joint transforms

init()

Initializes a collection of animatable transforms for a single skeletal pose.

init&lt;S>(S)

Initializes a collection of transforms of a specific type for a single skeletal pose.

init(arrayLiteral: Transform...)

Initializes a collection of animatable transforms using the argument elements for a single skeletal pose.

### Identifying joint transforms

typealias ArrayLiteralElement

The type of the elements of an array literal.

typealias Element

An individual joint transform in the collection.

typealias Index

A position of an individual joint transform in the collection.

typealias Indices

A type that represents the indices that are valid for subscripting the collection, in ascending order.

typealias Iterator

A type that provides the collection’s iteration interface and encapsulates its iteration state.

typealias SubSequence

A collection representing a contiguous subrange of this collection’s elements. The subsequence shares indices with the original collection.

### Inspecting joint transform details

var count: Int

The number of elements in the collection.

var first: Self.Element?

The first element of the collection.

var indices: DefaultIndices&lt;Self>

The indices that are valid for subscripting the collection, in ascending order.

var startIndex: JointTransforms.Index

An index to the first joint transform in the collection.

var endIndex: JointTransforms.Index

An index to the last joint transform in the collection.

var isEmpty: Bool

A Boolean value indicating whether the collection is empty.

var last: Self.Element?

The last element of the collection.

var lazy: LazySequence&lt;Self>

A sequence containing the same elements as this sequence, but on which some operations, such as `map` and `filter`, are implemented lazily.

var publisher: Publishers.Sequence&lt;Self, Never>

var underestimatedCount: Int

A value less than or equal to the number of elements in the collection.

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

func first(where: (Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the first element of the sequence that satisfies the given predicate.

func firstIndex(of: Self.Element) -> Self.Index?

Returns the first index where the specified value appears in the collection.

func firstIndex(where: (Self.Element) throws -> Bool) rethrows -> Self.Index?

Returns the first index in which an element of the collection satisfies the given predicate.

func flatMap&lt;SegmentOfResult>((Self.Element) throws -> SegmentOfResult) rethrows -> [SegmentOfResult.Element]

Returns an array containing the concatenated results of calling the given transformation with each element of this sequence.

func forEach((Self.Element) throws -> Void) rethrows

Calls the given closure on each element in the sequence in the same order as a `for`-`in` loop.

func formIndex(inout Self.Index, offsetBy: Int)

Offsets the given index by the specified distance.

func formIndex(inout Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Bool

Offsets the given index by the specified distance, or so that it equals the given limiting index.

func formIndex(after: inout Self.Index)

Replaces the given index with its successor.

func formIndex(before: inout Self.Index)

Replaces the given index with its predecessor.

func formatted&lt;S>(S) -> S.FormatOutput

func index(Self.Index, offsetBy: Int) -> Self.Index

func index(Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Self.Index?

func index(after: JointTransforms.Index) -> JointTransforms.Index

Returns the position in the sequence of the joint that follows the given position.

func index(before: JointTransforms.Index) -> JointTransforms.Index

Returns the position in the sequence of the joint that preceeds the given position.

func last(where: (Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the last element of the sequence that satisfies the given predicate.

func lastIndex(of: Self.Element) -> Self.Index?

Returns the last index where the specified value appears in the collection.

func lastIndex(where: (Self.Element) throws -> Bool) rethrows -> Self.Index?

Returns the index of the last element in the collection that matches the given predicate.

func lexicographicallyPrecedes&lt;OtherSequence>(OtherSequence, by: (Self.Element, Self.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether the sequence precedes another sequence in a lexicographical (dictionary) ordering, using the given predicate to compare elements.

func makeIterator() -> IndexingIterator&lt;Self>

Returns an iterator over the elements of the collection.

func map&lt;T, E>((Self.Element) throws(E) -> T) throws(E) -> [T]

Returns an array containing the results of mapping the given closure over the sequence’s elements.

func max(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the maximum element in the sequence, using the given predicate as the comparison between elements.

func min(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the minimum element in the sequence, using the given predicate as the comparison between elements.

func partition(by: (Self.Element) throws -> Bool) rethrows -> Self.Index

Reorders the elements of the collection such that all the elements that match the given predicate are after all the elements that don’t match.

func prefix(Int) -> Self.SubSequence

Returns a subsequence, up to the specified maximum length, containing the initial elements of the collection.

func prefix(through: Self.Index) -> Self.SubSequence

Returns a subsequence from the start of the collection through the specified position.

func prefix(upTo: Self.Index) -> Self.SubSequence

Returns a subsequence from the start of the collection up to, but not including, the specified position.

func prefix(while: (Self.Element) throws -> Bool) rethrows -> Self.SubSequence

Returns a subsequence containing the initial elements until `predicate` returns `false` and skipping the remaining elements.

func randomElement() -> Self.Element?

Returns a random element of the collection.

func randomElement&lt;T>(using: inout T) -> Self.Element?

Returns a random element of the collection, using the given generator as a source for randomness.

func reduce&lt;Result>(Result, (Result, Self.Element) throws -> Result) rethrows -> Result

Returns the result of combining the elements of the sequence using the given closure.

func reduce&lt;Result>(into: Result, (inout Result, Self.Element) throws -> ()) rethrows -> Result

Returns the result of combining the elements of the sequence using the given closure.

func reverse()

Reverses the elements of the collection in place.

func reversed() -> ReversedCollection&lt;Self>

Returns a view presenting the elements of the collection in reverse order.

func shuffled() -> [Self.Element]

Returns the elements of the sequence, shuffled.

func shuffled&lt;T>(using: inout T) -> [Self.Element]

Returns the elements of the sequence, shuffled using the given generator as a source for randomness.

func sorted(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> [Self.Element]

Returns the elements of the sequence, sorted using the given predicate as the comparison between elements.

func sorted&lt;Comparator>(using: Comparator) -> [Self.Element]

Returns the elements of the sequence, sorted using the given comparator to compare elements.

func sorted&lt;S, Comparator>(using: S) -> [Self.Element]

Returns the elements of the sequence, sorted using the given array of `SortComparator`s to compare elements.

func split(maxSplits: Int, omittingEmptySubsequences: Bool, whereSeparator: (Self.Element) throws -> Bool) rethrows -> [Self.SubSequence]

Returns the longest possible subsequences of the collection, in order, that don’t contain elements satisfying the given predicate.

func split(separator: Self.Element, maxSplits: Int, omittingEmptySubsequences: Bool) -> [Self.SubSequence]

Returns the longest possible subsequences of the collection, in order, around elements equal to the given element.

func starts&lt;PossiblePrefix>(with: PossiblePrefix) -> Bool

Returns a Boolean value indicating whether the initial elements of the sequence are the same as the elements in another sequence.

func starts&lt;PossiblePrefix>(with: PossiblePrefix, by: (Self.Element, PossiblePrefix.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether the initial elements of the sequence are equivalent to the elements in another sequence, using the given predicate as the equivalence test.

func suffix(Int) -> Self.SubSequence

Returns a subsequence, up to the given maximum length, containing the final elements of the collection.

func suffix(from: Self.Index) -> Self.SubSequence

Returns a subsequence from the specified position to the end of the collection.

func swapAt(Self.Index, Self.Index)

Exchanges the values at the specified indices of the collection.

func withContiguousMutableStorageIfAvailable&lt;R>((inout UnsafeMutableBufferPointer&lt;Self.Element>) throws -> R) rethrows -> R?

Executes a closure on the collection’s contiguous storage.

func withContiguousStorageIfAvailable&lt;R>((UnsafeBufferPointer&lt;Self.Element>) throws -> R) rethrows -> R?

Executes a closure on the sequence’s contiguous storage.

### Comparing joint transforms

static func == (JointTransforms, JointTransforms) -> Bool

Returns a Boolean value that indicates whether two collections of joints are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func compare&lt;Comparator>(Comparator.Compared, Comparator.Compared) -> ComparisonResult

If `lhs` is ordered before `rhs` in the ordering described by the given sequence of `SortComparator`s

### Deprecated

func flatMap&lt;ElementOfResult>((Self.Element) throws -> ElementOfResult?) rethrows -> [ElementOfResult]

func index(of: Self.Element) -> Self.Index?

Returns the first index where the specified value appears in the collection.

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

MutableCollection Implementations

Sequence Implementations

## Relationships

### Conforms To

- AnimatableData
- BidirectionalCollection
- Collection
- Copyable
- Decodable
- Encodable
- Equatable
- ExpressibleByArrayLiteral
- MutableCollection
- Sequence

