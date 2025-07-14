

- Combine
- Publishers
-  Publishers.TimeGroupingStrategy 

Enumeration

# Publishers.TimeGroupingStrategy

A strategy for collecting received elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum TimeGroupingStrategy where Context : Scheduler
```

## Topics

### Time Groupings

case byTime(Context, Context.SchedulerTimeType.Stride)

A grouping that collects and periodically publishes items.

case byTimeOrCount(Context, Context.SchedulerTimeType.Stride, Int)

A grouping that collects and publishes items periodically or when a buffer reaches a maximum size.

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

func reduce&lt;T>(T, (T, Self.Output) -> T) -> Publishers.Reduce&lt;Self, T>

Applies a closure that collects each element of a stream and publishes a final result upon completion.

func tryReduce&lt;T>(T, (T, Self.Output) throws -> T) -> Publishers.TryReduce&lt;Self, T>

Applies an error-throwing closure that collects each element of a stream and publishes a final result upon completion.

