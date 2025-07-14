

- Combine
- Publishers
- Publishers.TryReduce
-  collect() 

Instance Method

# collect()

Collects all received elements, and emits a single array of the collection when the upstream publisher finishes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func collect() -> Publishers.Collect
```

## Return Value

A publisher that collects all received items and returns them as an array upon completion.

## Discussion

Use collect() to gather elements into an array that the operator emits after the upstream publisher finishes.

If the upstream publisher fails with an error, this publisher forwards the error to the downstream receiver instead of sending its output.

This publisher requests an unlimited number of elements from the upstream publisher and uses an unbounded amount of memory to store the received values. The publisher may exert memory pressure on the system for very large sets of elements.

The collect() operator only sends the collected array to its downstream receiver after a request whose demand is greater than 0 items. Otherwise, collect() waits until it receives a non-zero request.

In the example below, an Integer range is a publisher that emits an array of integers:

```
let numbers = (0...10)
cancellable = numbers.publisher
    .collect()
    .sink { print("\($0)") }

// Prints: "[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]"
```

## See Also

### Reducing Elements

func collect(Int) -> Publishers.CollectByCount&lt;Self>

Collects up to the specified number of elements, and then emits a single array of the collection.

func collect&lt;S>(Publishers.TimeGroupingStrategy&lt;S>, options: S.SchedulerOptions?) -> Publishers.CollectByTime&lt;Self, S>

Collects elements by a given time-grouping strategy, and emits a single array of the collection.

func ignoreOutput() -> Publishers.IgnoreOutput&lt;Self>

Ignores all upstream elements, but passes along the upstream publisher’s completion state (finished or failed).

func reduce&lt;T>(T, (T, Self.Output) -> T) -> Publishers.Reduce&lt;Self, T>

Applies a closure that collects each element of a stream and publishes a final result upon completion.

func tryReduce&lt;T>(T, (T, Self.Output) throws -> T) -> Publishers.TryReduce&lt;Self, T>

Applies an error-throwing closure that collects each element of a stream and publishes a final result upon completion.

