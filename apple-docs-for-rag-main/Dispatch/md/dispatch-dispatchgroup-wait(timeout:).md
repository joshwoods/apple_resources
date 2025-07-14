

- Dispatch
- DispatchGroup
-  wait(timeout:) 

Instance Method

# wait(timeout:)

Waits synchronously for the previously submitted work to complete, and returns if the work is not completed before the specified timeout period has elapsed.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func wait(timeout: DispatchTime) -> DispatchTimeoutResult
```

## Parameters 

`timeout`  

The latest time to wait for a group to complete.

## Return Value

A result value indicating whether the method returned due to a timeout.

## See Also

### Waiting for Tasks to Finish Executing

func wait()

Waits synchronously for the previously submitted work to finish.

func wait(wallTimeout: DispatchWallTime) -> DispatchTimeoutResult

Waits synchronously for the previously submitted work to complete, and returns if the work is not completed before the specified timeout period has elapsed.

