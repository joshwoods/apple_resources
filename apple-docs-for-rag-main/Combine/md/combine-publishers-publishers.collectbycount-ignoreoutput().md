

- Combine
- Publishers
- Publishers.CollectByCount
-  ignoreOutput() 

Instance Method

# ignoreOutput()

Ignores all upstream elements, but passes along the upstream publisher’s completion state (finished or failed).

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func ignoreOutput() -> Publishers.IgnoreOutput
```

## Return Value

A publisher that ignores all upstream elements.

## Discussion

Use the ignoreOutput() operator to determine if a publisher is able to complete successfully or would fail.

In the example below, the array publisher (`numbers`) delivers the first five of its elements successfully, as indicated by the ignoreOutput() operator. The operator consumes, but doesn’t republish the elements downstream. However, the sixth element, `0`, causes the error throwing closure to catch a `NoZeroValuesAllowedError` that terminates the stream.

```
struct NoZeroValuesAllowedError: Error {}
let numbers = [1, 2, 3, 4, 5, 0, 6, 7, 8, 9]
cancellable = numbers.publisher
    .tryFilter({ anInt in
        guard anInt != 0 else { throw NoZeroValuesAllowedError() }
        return anInt 

The output type of this publisher is Never.

## See Also

### Reducing Elements

func collect() -> Publishers.Collect&lt;Self>

Collects all received elements, and emits a single array of the collection when the upstream publisher finishes.

func collect(Int) -> Publishers.CollectByCount&lt;Self>

Collects up to the specified number of elements, and then emits a single array of the collection.

func collect&lt;S>(Publishers.TimeGroupingStrategy&lt;S>, options: S.SchedulerOptions?) -> Publishers.CollectByTime&lt;Self, S>

Collects elements by a given time-grouping strategy, and emits a single array of the collection.

func reduce&lt;T>(T, (T, Self.Output) -> T) -> Publishers.Reduce&lt;Self, T>

Applies a closure that collects each element of a stream and publishes a final result upon completion.

func tryReduce&lt;T>(T, (T, Self.Output) throws -> T) -> Publishers.TryReduce&lt;Self, T>

Applies an error-throwing closure that collects each element of a stream and publishes a final result upon completion.

