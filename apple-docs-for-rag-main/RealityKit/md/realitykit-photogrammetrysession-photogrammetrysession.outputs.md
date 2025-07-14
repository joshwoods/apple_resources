

- RealityKit
- PhotogrammetrySession
-  PhotogrammetrySession.Outputs 

Structure

# PhotogrammetrySession.Outputs

An asynchronous sequence of session-related updates.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
struct Outputs
```

## Topics

### Iterating the collection

func makeAsyncIterator() -> PhotogrammetrySession.Outputs.Iterator

Creates an asynchronous iterator for the collection.

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

typealias Element

The type of element used for Photogrammetry Session updates.

struct Iterator

An object for iterating over published output objects.

### Filtering the output

func allSatisfy((Self.Element) async throws -> Bool) async rethrows -> Bool

Returns a Boolean value that indicates whether all elements produced by the asynchronous sequence satisfy the given predicate.

func compactMap&lt;ElementOfResult>((Self.Element) async throws -> ElementOfResult?) -> AsyncThrowingCompactMapSequence&lt;Self, ElementOfResult>

Creates an asynchronous sequence that maps an error-throwing closure over the base sequence’s elements, omitting results that don’t return a value.

func compactMap&lt;ElementOfResult>((Self.Element) async -> ElementOfResult?) -> AsyncCompactMapSequence&lt;Self, ElementOfResult>

Creates an asynchronous sequence that maps the given closure over the asynchronous sequence’s elements, omitting results that don’t return a value.

func contains(where: (Self.Element) async throws -> Bool) async rethrows -> Bool

Returns a Boolean value that indicates whether the asynchronous sequence contains an element that satisfies the given predicate.

func drop(while: (Self.Element) async -> Bool) -> AsyncDropWhileSequence&lt;Self>

Omits elements from the base asynchronous sequence until a given closure returns false, after which it passes through all remaining elements.

func dropFirst(Int) -> AsyncDropFirstSequence&lt;Self>

Omits a specified number of elements from the base asynchronous sequence, then passes through all remaining elements.

func filter((Self.Element) async -> Bool) -> AsyncFilterSequence&lt;Self>

Creates an asynchronous sequence that contains, in order, the elements of the base sequence that satisfy the given predicate.

func first(where: (Self.Element) async throws -> Bool) async rethrows -> Self.Element?

Returns the first element of the sequence that satisfies the given predicate.

func flatMap&lt;SegmentOfResult>((Self.Element) async throws -> SegmentOfResult) -> AsyncThrowingFlatMapSequence&lt;Self, SegmentOfResult>

Creates an asynchronous sequence that concatenates the results of calling the given error-throwing transformation with each element of this sequence.

func map&lt;Transformed>((Self.Element) async throws -> Transformed) -> AsyncThrowingMapSequence&lt;Self, Transformed>

Creates an asynchronous sequence that maps the given error-throwing closure over the asynchronous sequence’s elements.

func map&lt;Transformed>((Self.Element) async -> Transformed) -> AsyncMapSequence&lt;Self, Transformed>

Creates an asynchronous sequence that maps the given closure over the asynchronous sequence’s elements.

func prefix(Int) -> AsyncPrefixSequence&lt;Self>

Returns an asynchronous sequence, up to the specified maximum length, containing the initial elements of the base asynchronous sequence.

func prefix(while: (Self.Element) async -> Bool) rethrows -> AsyncPrefixWhileSequence&lt;Self>

Returns an asynchronous sequence, containing the initial, consecutive elements of the base sequence that satisfy the given predicate.

### Default Implementations

AsyncSequence Implementations

## Relationships

### Conforms To

- AsyncSequence

## See Also

### Iterating outputs

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

typealias Element

The type of element used for Photogrammetry Session updates.

