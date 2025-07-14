

- Swift
-  AsyncIteratorProtocol 

Protocol

# AsyncIteratorProtocol

A type that asynchronously supplies the values of a sequence one at a time.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol AsyncIteratorProtocol
```

## Overview

The `AsyncIteratorProtocol` defines the type returned by the `makeAsyncIterator()` method of the `AsyncSequence` protocol. In short, the iterator is what produces the asynchronous sequence’s values. The protocol defines a single asynchronous method, `next()`, which either produces the next element of the sequence, or returns `nil` to signal the end of the sequence.

To implement your own `AsyncSequence`, implement a wrapped type that conforms to `AsyncIteratorProtocol`. The following example shows a `Counter` type that uses an inner iterator to monotonically generate `Int` values until reaching a `howHigh` value. While this example isn’t itself asynchronous, it shows the shape of a custom sequence and iterator, and how to use it as if it were asynchronous:

```
struct Counter: AsyncSequence {
    typealias Element = Int
    let howHigh: Int

    struct AsyncIterator: AsyncIteratorProtocol {
        let howHigh: Int
        var current = 1

        mutating func next() async -> Int? {
            // A genuinely asynchronous implementation uses the `Task`
            // API to check for cancellation here and return early.
            guard current  AsyncIterator {
        return AsyncIterator(howHigh: howHigh)
    }
}
```

At the call site, this looks like:

```
for await number in Counter(howHigh: 10) {
  print(number, terminator: " ")
}
// Prints "1 2 3 4 5 6 7 8 9 10 "
```

### End of Iteration

The iterator returns `nil` to indicate the end of the sequence. After returning `nil` (or throwing an error) from `next()`, the iterator enters a terminal state, and all future calls to `next()` must return `nil`.

### Cancellation

Types conforming to `AsyncIteratorProtocol` should use the cancellation primitives provided by Swift’s `Task` API. The iterator can choose how to handle and respond to cancellation, including:

- Checking the `isCancelled` value of the current `Task` inside `next()` and returning `nil` to terminate the sequence.

- Calling `checkCancellation()` on the `Task`, which throws a `CancellationError`.

- Implementing `next()` with a `withTaskCancellationHandler(handler:operation:)` invocation to immediately react to cancellation.

If the iterator needs to clean up on cancellation, it can do so after checking for cancellation as described above, or in `deinit` if it’s a reference type.

## Topics

### Declaring Iterator Topography

associatedtype Element

**Required**

### Producing Iterator Values

func next() async throws -> Self.Element?

Asynchronously advances to the next element and returns it, or ends the sequence if there is no next element.

**Required** Default implementation provided.

### Associated Types

associatedtype Failure : Error = any Error

The type of failure produced by iteration.

**Required**

### Instance Methods

func next(isolation: isolated (any Actor)?) async throws(Self.Failure) -> Self.Element?

Asynchronously advances to the next element and returns it, or ends the sequence if there is no next element.

**Required** Default implementation provided.

## Relationships

### Conforming Types

- AsyncCompactMapSequence.Iterator

  Conforms when `Base` conforms to `AsyncSequence`.

- AsyncDropFirstSequence.Iterator

  Conforms when `Base` conforms to `AsyncSequence`.

- AsyncDropWhileSequence.Iterator

  Conforms when `Base` conforms to `AsyncSequence`.

- AsyncFilterSequence.Iterator

  Conforms when `Base` conforms to `AsyncSequence`.

- AsyncFlatMapSequence.Iterator

  Conforms when `Base` conforms to `AsyncSequence` and `SegmentOfResult` conforms to `AsyncSequence`.

- AsyncMapSequence.Iterator

  Conforms when `Base` conforms to `AsyncSequence`.

- AsyncPrefixSequence.Iterator

  Conforms when `Base` conforms to `AsyncSequence`.

- AsyncPrefixWhileSequence.Iterator

  Conforms when `Base` conforms to `AsyncSequence`.

- AsyncStream.Iterator
- AsyncThrowingCompactMapSequence.Iterator

  Conforms when `Base` conforms to `AsyncSequence`.

- AsyncThrowingDropWhileSequence.Iterator

  Conforms when `Base` conforms to `AsyncSequence`.

- AsyncThrowingFilterSequence.Iterator

  Conforms when `Base` conforms to `AsyncSequence`.

- AsyncThrowingFlatMapSequence.Iterator

  Conforms when `Base` conforms to `AsyncSequence` and `SegmentOfResult` conforms to `AsyncSequence`.

- AsyncThrowingMapSequence.Iterator

  Conforms when `Base` conforms to `AsyncSequence`.

- AsyncThrowingPrefixWhileSequence.Iterator

  Conforms when `Base` conforms to `AsyncSequence`.

- AsyncThrowingStream.Iterator

  Conforms when `Failure` conforms to `Error`.

- TaskGroup.Iterator

  Conforms when `ChildTaskResult` conforms to `Sendable`.

- ThrowingTaskGroup.Iterator

  Conforms when `ChildTaskResult` conforms to `Sendable` and `Failure` conforms to `Error`.

## See Also

### Creating an Iterator

func makeAsyncIterator() -> Self.AsyncIterator

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

**Required**

associatedtype AsyncIterator : AsyncIteratorProtocol

The type of asynchronous iterator that produces elements of this asynchronous sequence.

**Required**

associatedtype Element

The type of element produced by this asynchronous sequence.

**Required**

