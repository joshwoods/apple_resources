

- Dispatch
- DispatchSemaphore
-  signal() 

Instance Method

# signal()

Signals (increments) a semaphore.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
@discardableResult
func signal() -> Int
```

## Return Value

This function returns non-zero if a thread is woken. Otherwise, zero is returned.

## Discussion

Increment the counting semaphore. If the previous value was less than zero, this function wakes a thread currently waiting in dispatch_semaphore_wait.

