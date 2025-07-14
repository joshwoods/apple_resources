

- Swift
- TaskGroup
-  max() 

Instance Method

# max()

Returns the maximum element in an asynchronous sequence of comparable elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@warn_unqualified_access
func max() async rethrows -> Self.Element?
```

Available when `Element` conforms to `Comparable`.

## Return Value

The sequence’s maximum element. If the sequence has no elements, returns `nil`.

## Discussion

In this example, an asynchronous sequence called `Counter` produces `Int` values from `1` to `10`. The `max()` method returns the max value of the sequence.

```
let max = await Counter(howHigh: 10)
    .max()
print(max ?? "none")
// Prints "10"
```

## See Also

### Accessing an Asynchronous Sequence of Results

func makeAsyncIterator() -> TaskGroup&lt;ChildTaskResult>.Iterator

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

func allSatisfy((Self.Element) async throws -> Bool) async rethrows -> Bool

Returns a Boolean value that indicates whether all elements produced by the asynchronous sequence satisfy the given predicate.

func compactMap&lt;ElementOfResult>((Self.Element) async throws -> ElementOfResult?) -> AsyncThrowingCompactMapSequence&lt;Self, ElementOfResult>

Creates an asynchronous sequence that maps an error-throwing closure over the base sequence’s elements, omitting results that don’t return a value.

func compactMap&lt;ElementOfResult>((Self.Element) async -> ElementOfResult?) -> AsyncCompactMapSequence&lt;Self, ElementOfResult>

Creates an asynchronous sequence that maps the given closure over the asynchronous sequence’s elements, omitting results that don’t return a value.

func contains(Self.Element) async rethrows -> Bool

Returns a Boolean value that indicates whether the asynchronous sequence contains the given element.

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

func max(by: (Self.Element, Self.Element) async throws -> Bool) async rethrows -> Self.Element?

Returns the maximum element in the asynchronous sequence, using the given predicate as the comparison between elements.

func min() async rethrows -> Self.Element?

Returns the minimum element in an asynchronous sequence of comparable elements.

