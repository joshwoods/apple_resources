

- Dispatch
- DispatchWorkItem
-  wait(wallTimeout:) 

Instance Method

# wait(wallTimeout:)

Causes the caller to wait synchronously until the dispatch work item finishes executing, or until the specified time elapses.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.10+tvOSvisionOSwatchOS

``` source
func wait(wallTimeout: DispatchWallTime) -> DispatchTimeoutResult
```

## Parameters 

`wallTimeout`  

The time at which to stop waiting for the dispatch item to finish. Specifying distantFuture is equivalent to calling the wait() method.

## Return Value

DispatchTimeoutResult.success if the method returned because the work item finished executing, or DispatchTimeoutResult.timedOut if the timeout value was reached.

## Discussion

This method returns immediately if the current work item has already finished executing.

## See Also

### Waiting for the Completion of a Work Item

func wait()

Causes the caller to wait synchronously until the dispatch work item finishes executing.

func wait(timeout: DispatchTime) -> DispatchTimeoutResult

Causes the caller to wait synchronously until the dispatch work item finishes executing, or until the specified time elapses.

struct DispatchTime

A point in time relative to the default clock, with nanosecond precision.

struct DispatchWallTime

An absolute point in time according to the wall clock, with microsecond precision.

