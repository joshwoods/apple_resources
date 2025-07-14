

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Outputs
-  drop(while:) 

Instance Method

# drop(while:)

Omits elements from the base asynchronous sequence until a given closure returns false, after which it passes through all remaining elements.

RealityKitSwiftiOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
@preconcurrency
func drop(while predicate: @escaping (Self.Element) async -> Bool) -> AsyncDropWhileSequence
```

## Parameters 

`predicate`  

A closure that takes an element as a parameter and returns a Boolean value indicating whether to drop the element from the modified sequence.

## Return Value

An asynchronous sequence that skips over values from the base sequence until the provided closure returns `false`.

## Discussion

Use `drop(while:)` to omit elements from an asynchronous sequence until the element received meets a condition you specify.

In this example, an asynchronous sequence called `Counter` produces `Int` values from `1` to `10`. The `drop(while:)` method causes the modified sequence to ignore received values until it encounters one that is divisible by `3`:

```
let stream = Counter(howHigh: 10)
    .drop { $0 % 3 != 0 }
for await number in stream {
    print(number, terminator: " ")
}
// Prints "3 4 5 6 7 8 9 10 "
```

After the predicate returns `false`, the sequence never executes it again, and from then on the sequence passes through elements from its underlying sequence as-is.

## See Also

### Filtering the output

func allSatisfy((Self.Element) async throws -> Bool) async rethrows -> Bool

Returns a Boolean value that indicates whether all elements produced by the asynchronous sequence satisfy the given predicate.

func compactMap&lt;ElementOfResult>((Self.Element) async throws -> ElementOfResult?) -> AsyncThrowingCompactMapSequence&lt;Self, ElementOfResult>

Creates an asynchronous sequence that maps an error-throwing closure over the base sequence’s elements, omitting results that don’t return a value.

func compactMap&lt;ElementOfResult>((Self.Element) async -> ElementOfResult?) -> AsyncCompactMapSequence&lt;Self, ElementOfResult>

Creates an asynchronous sequence that maps the given closure over the asynchronous sequence’s elements, omitting results that don’t return a value.

func contains(where: (Self.Element) async throws -> Bool) async rethrows -> Bool

Returns a Boolean value that indicates whether the asynchronous sequence contains an element that satisfies the given predicate.

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

