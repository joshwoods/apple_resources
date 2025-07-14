

- RealityKit
-  QueryResult 

Structure

# QueryResult

An object that returns the results of an entity query.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct QueryResult
```

## Overview

You can’t create query result objects. Instead, call performQuery(_:), which returns a QueryResult containing the entities that meet your specified query criteria.

```
// Ask the scene to perform the query and iterate over the returned entities.
scene.performQuery(query).forEach { entity in
    print("Returned entity: \(entity)")
}
```

## Topics

### Creating an iterator

struct Iterator

The type of iterator used for entity query results.

func makeIterator() -> QueryResult&lt;Element>.Iterator

Returns an iterator for the contained entities.

### Finding elements

func contains(Self.Element) -> Bool

Returns a Boolean value indicating whether the sequence contains the given element.

func contains(where: (Self.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether the sequence contains an element that satisfies the given predicate.

func allSatisfy((Self.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether every element of a sequence satisfies a given predicate.

func max(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the maximum element in the sequence, using the given predicate as the comparison between elements.

### Selecting elements

func prefix(Int) -> PrefixSequence&lt;Self>

Returns a sequence, up to the specified maximum length, containing the initial elements of the sequence.

func prefix(while: (Self.Element) throws -> Bool) rethrows -> [Self.Element]

Returns a sequence containing the initial, consecutive elements that satisfy the given predicate.

func suffix(Int) -> [Self.Element]

Returns a subsequence, up to the given maximum length, containing the final elements of the sequence.

### Excluding elements

func drop(while: (Self.Element) throws -> Bool) rethrows -> DropWhileSequence&lt;Self>

Returns a sequence by skipping the initial, consecutive elements that satisfy the given predicate.

func filter((Self.Element) throws -> Bool) rethrows -> [Self.Element]

Returns an array containing, in order, the elements of the sequence that satisfy the given predicate.

func filter&lt;T>(matchingCategory: CMTypedTag&lt;T>.Category) -> [CMTypedTag&lt;T>]

Filters a sequence of tags based on matching the specified category. Returns the tags that match the specified category.

### Transforming a sequence

func map&lt;T, E>((Self.Element) throws(E) -> T) throws(E) -> [T]

Returns an array containing the results of mapping the given closure over the sequence’s elements.

func flatMap&lt;SegmentOfResult>((Self.Element) throws -> SegmentOfResult) rethrows -> [SegmentOfResult.Element]

Returns an array containing the concatenated results of calling the given transformation with each element of this sequence.

func compactMap&lt;ElementOfResult>((Self.Element) throws -> ElementOfResult?) rethrows -> [ElementOfResult]

Returns an array containing the non-`nil` results of calling the given transformation with each element of this sequence.

func reduce&lt;Result>(Result, (Result, Self.Element) throws -> Result) rethrows -> Result

Returns the result of combining the elements of the sequence using the given closure.

func reduce&lt;Result>(into: Result, (inout Result, Self.Element) throws -> ()) rethrows -> Result

Returns the result of combining the elements of the sequence using the given closure.

var lazy: LazySequence&lt;Self>

A sequence containing the same elements as this sequence, but on which some operations, such as `map` and `filter`, are implemented lazily.

func flatMap&lt;ElementOfResult>((Self.Element) throws -> ElementOfResult?) rethrows -> [ElementOfResult]

### Iterating over a sequence’s elements

func forEach((Self.Element) throws -> Void) rethrows

Calls the given closure on each element in the sequence in the same order as a `for`-`in` loop.

func enumerated() -> EnumeratedSequence&lt;Self>

Returns a sequence of pairs (*n*, *x*), where *n* represents a consecutive integer starting at zero and *x* represents an element of the sequence.

var underestimatedCount: Int

A value less than or equal to the number of elements in the sequence, calculated nondestructively.

### Reordering elements

func shuffled() -> [Self.Element]

Returns the elements of the sequence, shuffled.

func shuffled&lt;T>(using: inout T) -> [Self.Element]

Returns the elements of the sequence, shuffled using the given generator as a source for randomness.

### Splitting and joining elements

func split(maxSplits: Int, omittingEmptySubsequences: Bool, whereSeparator: (Self.Element) throws -> Bool) rethrows -> [ArraySlice&lt;Self.Element>]

Returns the longest possible subsequences of the sequence, in order, that don’t contain elements satisfying the given predicate. Elements that are used to split the sequence are not returned as part of any subsequence.

func split(separator: Self.Element, maxSplits: Int, omittingEmptySubsequences: Bool) -> [ArraySlice&lt;Self.Element>]

Returns the longest possible subsequences of the sequence, in order, around elements equal to the given element.

func joined() -> FlattenSequence&lt;Self>

Returns the elements of this sequence of sequences, concatenated.

func joined&lt;Separator>(separator: Separator) -> JoinedSequence&lt;Self>

Returns the concatenated elements of this sequence of sequences, inserting the given separator between each element.

func joined(separator: String) -> String

Returns a new string by concatenating the elements of the sequence, adding the given separator between each element.

### Comparing sequences

func elementsEqual&lt;OtherSequence>(OtherSequence) -> Bool

Returns a Boolean value indicating whether this sequence and another sequence contain the same elements in the same order.

func elementsEqual&lt;OtherSequence>(OtherSequence, by: (Self.Element, OtherSequence.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether this sequence and another sequence contain equivalent elements in the same order, using the given predicate as the equivalence test.

func starts&lt;PossiblePrefix>(with: PossiblePrefix) -> Bool

Returns a Boolean value indicating whether the initial elements of the sequence are the same as the elements in another sequence.

func starts&lt;PossiblePrefix>(with: PossiblePrefix, by: (Self.Element, PossiblePrefix.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether the initial elements of the sequence are equivalent to the elements in another sequence, using the given predicate as the equivalence test.

### Accessing underlying storage

func withContiguousStorageIfAvailable&lt;R>((UnsafeBufferPointer&lt;Self.Element>) throws -> R) rethrows -> R?

Executes a closure on the sequence’s contiguous storage.

### Publishing a sequence

var publisher: Publishers.Sequence&lt;Self, Never>

### Default Implementations

Sequence Implementations

## Relationships

### Conforms To

- Copyable
- Sequence

## See Also

### Entity queries

struct EntityQuery

An object that retrieves entities from a scene.

struct QueryPredicate

An object that defines the criteria for an entity query.

