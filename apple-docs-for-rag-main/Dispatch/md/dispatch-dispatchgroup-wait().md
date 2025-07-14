

- Dispatch
- DispatchGroup
-  wait() 

Instance Method

# wait()

Waits synchronously for the previously submitted work to finish.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func wait()
```

## See Also

### Waiting for Tasks to Finish Executing

func wait(timeout: DispatchTime) -> DispatchTimeoutResult

Waits synchronously for the previously submitted work to complete, and returns if the work is not completed before the specified timeout period has elapsed.

func wait(wallTimeout: DispatchWallTime) -> DispatchTimeoutResult

Waits synchronously for the previously submitted work to complete, and returns if the work is not completed before the specified timeout period has elapsed.

