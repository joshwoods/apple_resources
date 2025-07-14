

- Swift
- AsyncSequence
-  reduce(\_:\_:) 

Instance Method

# reduce(\_:\_:)

Returns the result of combining the elements of the asynchronous sequence using the given closure.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func reduce(
    _ initialResult: Result,
    _ nextPartialResult: (Result, Self.Element) async throws -> Result
) async rethrows -> Result
```

## Parameters 

`initialResult`  

The value to use as the initial accumulating value. The `nextPartialResult` closure receives `initialResult` the first time the closure runs.

`nextPartialResult`  

A closure that combines an accumulating value and an element of the asynchronous sequence into a new accumulating value, for use in the next call of the `nextPartialResult` closure or returned to the caller.

## Return Value

The final accumulated value. If the sequence has no elements, the result is `initialResult`.

## Discussion

Use the `reduce(_:_:)` method to produce a single value from the elements of an entire sequence. For example, you can use this method on an sequence of numbers to find their sum or product.

The `nextPartialResult` closure executes sequentially with an accumulating value initialized to `initialResult` and each element of the sequence.

In this example, an asynchronous sequence called `Counter` produces `Int` values from `1` to `4`. The `reduce(_:_:)` method sums the values received from the asynchronous sequence.

```
let sum = await Counter(howHigh: 4)
    .reduce(0) {
        $0 + $1
    }
print(sum)
// Prints "10"
```

## See Also

### Transforming a Sequence

func map&lt;Transformed>((Self.Element) async -> Transformed) -> AsyncMapSequence&lt;Self, Transformed>

Creates an asynchronous sequence that maps the given closure over the asynchronous sequence’s elements.

struct AsyncMapSequence

An asynchronous sequence that maps the given closure over the asynchronous sequence’s elements.

func map&lt;Transformed>((Self.Element) async throws -> Transformed) -> AsyncThrowingMapSequence&lt;Self, Transformed>

Creates an asynchronous sequence that maps the given error-throwing closure over the asynchronous sequence’s elements.

struct AsyncThrowingMapSequence

An asynchronous sequence that maps the given error-throwing closure over the asynchronous sequence’s elements.

func compactMap&lt;ElementOfResult>((Self.Element) async -> ElementOfResult?) -> AsyncCompactMapSequence&lt;Self, ElementOfResult>

Creates an asynchronous sequence that maps the given closure over the asynchronous sequence’s elements, omitting results that don’t return a value.

struct AsyncCompactMapSequence

An asynchronous sequence that maps a given closure over the asynchronous sequence’s elements, omitting results that don’t return a value.

func compactMap&lt;ElementOfResult>((Self.Element) async throws -> ElementOfResult?) -> AsyncThrowingCompactMapSequence&lt;Self, ElementOfResult>

Creates an asynchronous sequence that maps an error-throwing closure over the base sequence’s elements, omitting results that don’t return a value.

struct AsyncThrowingCompactMapSequence

An asynchronous sequence that maps an error-throwing closure over the base sequence’s elements, omitting results that don’t return a value.

struct AsyncFlatMapSequence

An asynchronous sequence that concatenates the results of calling a given transformation with each element of this sequence.

struct AsyncThrowingFlatMapSequence

An asynchronous sequence that concatenates the results of calling a given error-throwing transformation with each element of this sequence.

func reduce&lt;Result>(into: Result, (inout Result, Self.Element) async throws -> Void) async rethrows -> Result

Returns the result of combining the elements of the asynchronous sequence using the given closure, given a mutable initial value.

