

- Dispatch
- DispatchGroup
-  wait(wallTimeout:) 

Instance Method

# wait(wallTimeout:)

Waits synchronously for the previously submitted work to complete, and returns if the work is not completed before the specified timeout period has elapsed.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func wait(wallTimeout timeout: DispatchWallTime) -> DispatchTimeoutResult
```

## Parameters 

`timeout`  

The latest time to wait for a group to complete.

## Return Value

DispatchTimeoutResult.timedOut if the method returned due to a timeout, or DispatchTimeoutResult.success if the tasks completed.

## See Also

### Waiting for Tasks to Finish Executing

func wait()

Waits synchronously for the previously submitted work to finish.

func wait(timeout: DispatchTime) -> DispatchTimeoutResult

Waits synchronously for the previously submitted work to complete, and returns if the work is not completed before the specified timeout period has elapsed.

