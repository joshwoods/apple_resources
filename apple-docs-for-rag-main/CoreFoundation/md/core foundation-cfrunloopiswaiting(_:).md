

- Core Foundation
-  CFRunLoopIsWaiting(\_:) 

Function

# CFRunLoopIsWaiting(\_:)

Returns a Boolean value that indicates whether the run loop is waiting for an event.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFRunLoopIsWaiting(_ rl: CFRunLoop!) -> Bool
```

## Parameters 

`rl`  

The run loop to examine.

## Return Value

`true` if `rl` has no events to process and is blocking, waiting for a source or timer to become ready to fire; `false` if `rl` either is not running or is currently processing a source, timer, or observer.

## Discussion

This function is useful only to test the state of another thread’s run loop. When called with the current thread’s run loop, this function always returns `false`.

## See Also

### Starting and Stopping a Run Loop

func CFRunLoopRun()

Runs the current thread’s CFRunLoop object in its default mode indefinitely.

func CFRunLoopRunInMode(CFRunLoopMode!, CFTimeInterval, Bool) -> CFRunLoopRunResult

Runs the current thread’s CFRunLoop object in a particular mode.

func CFRunLoopWakeUp(CFRunLoop!)

Wakes a waiting CFRunLoop object.

func CFRunLoopStop(CFRunLoop!)

Forces a CFRunLoop object to stop running.

