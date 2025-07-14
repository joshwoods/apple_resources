

- Dispatch
- DispatchSemaphore
-  wait(timeout:) 

Instance Method

# wait(timeout:)

Waits for, or decrements, a semaphore.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func wait(timeout: DispatchTime) -> DispatchTimeoutResult
```

## Parameters 

`timeout`  

The latest time to wait for a signal.

## Discussion

Decrement the counting semaphore. If the resulting value is less than zero, this function waits for a signal to occur before returning.

## See Also

### Blocking on the Semaphore

func wait()

Waits for, or decrements, a semaphore.

func wait(wallTimeout: DispatchWallTime) -> DispatchTimeoutResult

Waits for, or decrements, a semaphore.

