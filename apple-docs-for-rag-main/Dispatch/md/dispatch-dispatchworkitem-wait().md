

- Dispatch
- DispatchWorkItem
-  wait() 

Instance Method

# wait()

Causes the caller to wait synchronously until the dispatch work item finishes executing.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.10+tvOSvisionOSwatchOS

``` source
func wait()
```

## Discussion

This method returns immediately if the current work item has already finished executing.

## See Also

### Waiting for the Completion of a Work Item

func wait(timeout: DispatchTime) -> DispatchTimeoutResult

Causes the caller to wait synchronously until the dispatch work item finishes executing, or until the specified time elapses.

func wait(wallTimeout: DispatchWallTime) -> DispatchTimeoutResult

Causes the caller to wait synchronously until the dispatch work item finishes executing, or until the specified time elapses.

struct DispatchTime

A point in time relative to the default clock, with nanosecond precision.

struct DispatchWallTime

An absolute point in time according to the wall clock, with microsecond precision.

