

- Core Motion
- CMStepCounter
-  queryStepCountStarting(from:to:to:withHandler:) Deprecated

Instance Method

# queryStepCountStarting(from:to:to:withHandler:)

Gathers and returns historical step count data for the specified time period.

iOS 7.0–8.0DeprecatediPadOS 7.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func queryStepCountStarting(
    from start: Date,
    to end: Date,
    to queue: OperationQueue,
    withHandler handler: @escaping CMStepQueryHandler
)
```

Deprecated

Use CMPedometer instead

## Parameters 

`start`  

The start time to use when gathering step count data. This parameter must not be `nil`.

`end`  

The end time to use when gathering step count data. This parameter must not be `nil`.

`queue`  

The operation queue on which to execute the specified `handler` block. You can specify a custom queue or use the operation queue associated with your app’s main thread. This parameter must not be `nil`.

`handler`  

The block to execute with the results. For information about the parameters of this block, see CMStepQueryHandler. This parameter must not be `nil`.

## Discussion

This method runs asynchronously, returning immediately and delivering the results to the specified `handler` block. The system stores only the last seven days worth of step data at most. If there are no samples for the specified range of time, a value of 0 is passed to the `handler` block.

## See Also

### Getting Historical Step Counting Data

typealias CMStepQueryHandler

A block that reports the number of steps for a query operation.

