

- Combine
- Just
-  tryReduce(\_:\_:) 

Instance Method

# tryReduce(\_:\_:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func tryReduce(
    _ initialResult: T,
    _ nextPartialResult: (T, Output) throws -> T
) -> Result.Publisher
```

## See Also

### Reducing Elements

func collect() -> Just&lt;[Output]>

func collect(Int) -> Publishers.CollectByCount&lt;Self>

Collects up to the specified number of elements, and then emits a single array of the collection.

func collect&lt;S>(Publishers.TimeGroupingStrategy&lt;S>, options: S.SchedulerOptions?) -> Publishers.CollectByTime&lt;Self, S>

Collects elements by a given time-grouping strategy, and emits a single array of the collection.

func ignoreOutput() -> Empty&lt;Output, Just&lt;Output>.Failure>

func reduce&lt;T>(T, (T, Output) -> T) -> Result&lt;T, Just&lt;Output>.Failure>.Publisher

