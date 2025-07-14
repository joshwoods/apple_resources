

- Core Foundation
-  CFRunLoopRun() 

Function

# CFRunLoopRun()

Runs the current thread’s CFRunLoop object in its default mode indefinitely.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFRunLoopRun()
```

## Discussion

The current thread’s run loop runs in the default mode (see Default Run Loop Mode) until the run loop is stopped with CFRunLoopStop(_:) or all the sources and timers are removed from the default run loop mode.

Run loops can be run recursively. You can call CFRunLoopRun() from within any run loop callout and create nested run loop activations on the current thread’s call stack.

## See Also

### Starting and Stopping a Run Loop

func CFRunLoopRunInMode(CFRunLoopMode!, CFTimeInterval, Bool) -> CFRunLoopRunResult

Runs the current thread’s CFRunLoop object in a particular mode.

func CFRunLoopWakeUp(CFRunLoop!)

Wakes a waiting CFRunLoop object.

func CFRunLoopStop(CFRunLoop!)

Forces a CFRunLoop object to stop running.

func CFRunLoopIsWaiting(CFRunLoop!) -> Bool

Returns a Boolean value that indicates whether the run loop is waiting for an event.

