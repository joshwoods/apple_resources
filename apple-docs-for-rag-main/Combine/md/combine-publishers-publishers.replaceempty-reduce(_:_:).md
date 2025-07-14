

- Combine
- Publishers
- Publishers.ReplaceEmpty
-  reduce(\_:\_:) 

Instance Method

# reduce(\_:\_:)

Applies a closure that collects each element of a stream and publishes a final result upon completion.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func reduce(
    _ initialResult: T,
    _ nextPartialResult: @escaping (T, Self.Output) -> T
) -> Publishers.Reduce
```

## Parameters 

`initialResult`  

The value that the closure receives the first time it’s called.

`nextPartialResult`  

A closure that produces a new value by taking the previously-accumulated value and the next element it receives from the upstream publisher.

## Return Value

A publisher that applies the closure to all received elements and produces an accumulated value when the upstream publisher finishes. If reduce(_:_:) receives an error from the upstream publisher, the operator delivers it to the downstream subscriber, the publisher terminates and publishes no value.

## Discussion

Use reduce(_:_:) to collect a stream of elements and produce an accumulated value based on a closure you provide.

In the following example, the reduce(_:_:) operator collects all the integer values it receives from its upstream publisher:

```
let numbers = (0...10)
cancellable = numbers.publisher
    .reduce(0, { accum, next in accum + next })
    .sink { print("\($0)") }

// Prints: "55"
```

## See Also

### Reducing Elements

func collect() -> Publishers.Collect&lt;Self>

Collects all received elements, and emits a single array of the collection when the upstream publisher finishes.

func collect(Int) -> Publishers.CollectByCount&lt;Self>

Collects up to the specified number of elements, and then emits a single array of the collection.

func collect&lt;S>(Publishers.TimeGroupingStrategy&lt;S>, options: S.SchedulerOptions?) -> Publishers.CollectByTime&lt;Self, S>

Collects elements by a given time-grouping strategy, and emits a single array of the collection.

func ignoreOutput() -> Publishers.IgnoreOutput&lt;Self>

Ignores all upstream elements, but passes along the upstream publisher’s completion state (finished or failed).

func tryReduce&lt;T>(T, (T, Self.Output) throws -> T) -> Publishers.TryReduce&lt;Self, T>

Applies an error-throwing closure that collects each element of a stream and publishes a final result upon completion.

