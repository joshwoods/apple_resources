

- Core Motion
- CMMotionActivityManager
-  queryActivityStarting(from:to:to:withHandler:) 

Instance Method

# queryActivityStarting(from:to:to:withHandler:)

Gathers and returns historical motion data for the specified time period

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+watchOS 2.0+

``` source
func queryActivityStarting(
    from start: Date,
    to end: Date,
    to queue: OperationQueue,
    withHandler handler: @escaping CMMotionActivityQueryHandler
)
```

## Parameters 

`start`  

The start time to use when gathering motion data. This parameter must not be `nil`.

`end`  

The end time to use when gathering motion data. This parameter must not be `nil`.

`queue`  

The operation queue on which to execute the specified `handler` block. You can specify a custom queue or use the operation queue associated with your app’s main thread. This parameter must not be `nil`.

`handler`  

The block to execute with the results. For information about the parameters of this block, see CMMotionActivityQueryHandler. This parameter must not be `nil`.

## Discussion

This method runs asynchronously, returning immediately and delivering the results to the specified `handler` block. A delay of up to several minutes in reported activities is expected.

The system stores only the last seven days worth of activity data at most. If there are no samples for the specified range of time, an error object with the code CMErrorUnknown is passed to the `handler` block.

## See Also

### Getting Historical Activity Data

typealias CMMotionActivityQueryHandler

A block that reports the motion updates that occurred between the specified query interval.

