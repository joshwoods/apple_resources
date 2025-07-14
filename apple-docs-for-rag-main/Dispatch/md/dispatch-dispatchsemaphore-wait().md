

- Dispatch
- DispatchSemaphore
-  wait() 

Instance Method

# wait()

Waits for, or decrements, a semaphore.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func wait()
```

## Discussion

Decrement the counting semaphore. If the resulting value is less than zero, this function waits for a signal to occur before returning.

## See Also

### Blocking on the Semaphore

func wait(timeout: DispatchTime) -> DispatchTimeoutResult

Waits for, or decrements, a semaphore.

func wait(wallTimeout: DispatchWallTime) -> DispatchTimeoutResult

Waits for, or decrements, a semaphore.

