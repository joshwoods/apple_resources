

- Create ML
- MLDataTable
- 
  - MLDataTable
- MLDataTable.Rows
- MLDataTable.Row
- MLDataTable.Row.Values
-  Sequence Implementations 

API Collection

# Sequence Implementations

## Topics

### Instance Properties

var lazy: LazySequence&lt;Self>

A sequence containing the same elements as this sequence, but on which some operations, such as `map` and `filter`, are implemented lazily.

var publisher: Publishers.Sequence&lt;Self, Never>

### Instance Methods

func allSatisfy((Self.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether every element of a sequence satisfies a given predicate.

func compactMap&lt;ElementOfResult>((Self.Element) throws -> ElementOfResult?) rethrows -> [ElementOfResult]

Returns an array containing the non-`nil` results of calling the given transformation with each element of this sequence.

func compare&lt;Comparator>(Comparator.Compared, Comparator.Compared) -> ComparisonResult

If `lhs` is ordered before `rhs` in the ordering described by the given sequence of `SortComparator`s

func contains(Self.Element) -> Bool

Returns a Boolean value indicating whether the sequence contains the given element.

func contains(where: (Self.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether the sequence contains an element that satisfies the given predicate.

func count&lt;E>(where: (Self.Element) throws(E) -> Bool) throws(E) -> Int

Returns the number of elements in the sequence that satisfy the given predicate.

func elementsEqual&lt;OtherSequence>(OtherSequence) -> Bool

Returns a Boolean value indicating whether this sequence and another sequence contain the same elements in the same order.

func elementsEqual&lt;OtherSequence>(OtherSequence, by: (Self.Element, OtherSequence.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether this sequence and another sequence contain equivalent elements in the same order, using the given predicate as the equivalence test.

func enumerated() -> EnumeratedSequence&lt;Self>

Returns a sequence of pairs (*n*, *x*), where *n* represents a consecutive integer starting at zero and *x* represents an element of the sequence.

func filter(Predicate&lt;Self.Element>) throws -> [Self.Element]

func filter((Self.Element) throws -> Bool) rethrows -> [Self.Element]

Returns an array containing, in order, the elements of the sequence that satisfy the given predicate.

func first(where: (Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the first element of the sequence that satisfies the given predicate.

func flatMap&lt;ElementOfResult>((Self.Element) throws -> ElementOfResult?) rethrows -> [ElementOfResult]

func flatMap&lt;SegmentOfResult>((Self.Element) throws -> SegmentOfResult) rethrows -> [SegmentOfResult.Element]

Returns an array containing the concatenated results of calling the given transformation with each element of this sequence.

func forEach((Self.Element) throws -> Void) rethrows

Calls the given closure on each element in the sequence in the same order as a `for`-`in` loop.

func formatted&lt;S>(S) -> S.FormatOutput

func lexicographicallyPrecedes&lt;OtherSequence>(OtherSequence, by: (Self.Element, Self.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether the sequence precedes another sequence in a lexicographical (dictionary) ordering, using the given predicate to compare elements.

func map&lt;T, E>((Self.Element) throws(E) -> T) throws(E) -> [T]

Returns an array containing the results of mapping the given closure over the sequence’s elements.

func mapAnnotations&lt;Feature, Input, Output>((Input) throws -> Output) rethrows -> [AnnotatedFeature&lt;Feature, Output>]

Returns an array containing the results of mapping the given closure over the sequence’s annotations.

func mapAnnotations&lt;Feature, Input, Output>((Input) async throws -> Output) async rethrows -> [AnnotatedFeature&lt;Feature, Output>]

Returns an array containing the results of mapping the given async closure over the sequence’s annotations.

func mapFeatures&lt;Input, Output, Annotation>((Input) async throws -> Output) async rethrows -> [AnnotatedFeature&lt;Output, Annotation>]

Returns an array containing the results of mapping the given async closure over the sequence’s features.

func mapFeatures&lt;Input, Output, Annotation>((Input) throws -> Output) rethrows -> [AnnotatedFeature&lt;Output, Annotation>]

Returns an array containing the results of mapping the given closure over the sequence’s features.

func max(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the maximum element in the sequence, using the given predicate as the comparison between elements.

func min(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the minimum element in the sequence, using the given predicate as the comparison between elements.

func randomSplit&lt;T>(by: Double, seed: Int?) -> (ArraySlice&lt;T>, ArraySlice&lt;T>)

Generates two generic arrays by randomly splitting the elements of the sequence.

func randomSplit&lt;Feature, Annotation>(by: Double, seed: Int?) -> ([AnnotatedFeature&lt;Feature, Annotation>], [AnnotatedFeature&lt;Feature, Annotation>])

Generates two AnnotatedFeatures by randomly splitting the elements of the sequence, at the same proportion within each unique Annotation.

func randomSplit&lt;T, Generator>(by: Double, using: inout Generator) -> (ArraySlice&lt;T>, ArraySlice&lt;T>)

Generates two generic arrays by randomly splitting the elements of the sequence.

func randomSplit&lt;Feature, Annotation, Generator>(by: Double, using: inout Generator) -> ([AnnotatedFeature&lt;Feature, Annotation>], [AnnotatedFeature&lt;Feature, Annotation>])

Generates two AnnotatedFeatures by randomly splitting the elements of the sequence, at the same proportion within each unique Annotation.

func reduce&lt;Result>(Result, (Result, Self.Element) throws -> Result) rethrows -> Result

Returns the result of combining the elements of the sequence using the given closure.

func reduce&lt;Result>(into: Result, (inout Result, Self.Element) throws -> ()) rethrows -> Result

Returns the result of combining the elements of the sequence using the given closure.

func shuffled() -> [Self.Element]

Returns the elements of the sequence, shuffled.

func shuffled&lt;T>(using: inout T) -> [Self.Element]

Returns the elements of the sequence, shuffled using the given generator as a source for randomness.

func sorted(by: (Self.Element, Self.Element) throws -> Bool) rethrows -> [Self.Element]

Returns the elements of the sequence, sorted using the given predicate as the comparison between elements.

func sorted&lt;S, Comparator>(using: S) -> [Self.Element]

Returns the elements of the sequence, sorted using the given array of `SortComparator`s to compare elements.

func sorted&lt;Comparator>(using: Comparator) -> [Self.Element]

Returns the elements of the sequence, sorted using the given comparator to compare elements.

func starts&lt;PossiblePrefix>(with: PossiblePrefix) -> Bool

Returns a Boolean value indicating whether the initial elements of the sequence are the same as the elements in another sequence.

func starts&lt;PossiblePrefix>(with: PossiblePrefix, by: (Self.Element, PossiblePrefix.Element) throws -> Bool) rethrows -> Bool

Returns a Boolean value indicating whether the initial elements of the sequence are equivalent to the elements in another sequence, using the given predicate as the equivalence test.

func withContiguousStorageIfAvailable&lt;R>((UnsafeBufferPointer&lt;Self.Element>) throws -> R) rethrows -> R?

Executes a closure on the sequence’s contiguous storage.

