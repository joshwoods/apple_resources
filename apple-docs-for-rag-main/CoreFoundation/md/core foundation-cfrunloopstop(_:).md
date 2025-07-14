

- Core Foundation
-  CFRunLoopStop(\_:) 

Function

# CFRunLoopStop(\_:)

Forces a CFRunLoop object to stop running.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFRunLoopStop(_ rl: CFRunLoop!)
```

## Parameters 

`rl`  

The run loop to stop.

## Discussion

This function forces `rl` to stop running and return control to the function that called CFRunLoopRun() or CFRunLoopRunInMode(_:_:_:) for the current run loop activation. If the run loop is nested with a callout from one activation starting another activation running, only the innermost activation is exited.

## See Also

### Starting and Stopping a Run Loop

func CFRunLoopRun()

Runs the current thread’s CFRunLoop object in its default mode indefinitely.

func CFRunLoopRunInMode(CFRunLoopMode!, CFTimeInterval, Bool) -> CFRunLoopRunResult

Runs the current thread’s CFRunLoop object in a particular mode.

func CFRunLoopWakeUp(CFRunLoop!)

Wakes a waiting CFRunLoop object.

func CFRunLoopIsWaiting(CFRunLoop!) -> Bool

Returns a Boolean value that indicates whether the run loop is waiting for an event.

