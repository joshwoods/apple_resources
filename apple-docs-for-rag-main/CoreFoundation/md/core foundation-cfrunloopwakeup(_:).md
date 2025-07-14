

- Core Foundation
-  CFRunLoopWakeUp(\_:) 

Function

# CFRunLoopWakeUp(\_:)

Wakes a waiting CFRunLoop object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFRunLoopWakeUp(_ rl: CFRunLoop!)
```

## Parameters 

`rl`  

The run loop to wake up.

## Discussion

A run loop goes to sleep when it is waiting for a source or timer to become ready to fire. If no source or timer fires, the run loop stays there until it times out or is explicitly woken up. If a run loop is modified, such as a new source added, you need to wake up the run loop to allow it to process the change. Version 0 sources use CFRunLoopWakeUp(_:) to cause the run loop to wake up after setting a source to be signaled, if they want the source handled immediately.

## See Also

### Starting and Stopping a Run Loop

func CFRunLoopRun()

Runs the current thread’s CFRunLoop object in its default mode indefinitely.

func CFRunLoopRunInMode(CFRunLoopMode!, CFTimeInterval, Bool) -> CFRunLoopRunResult

Runs the current thread’s CFRunLoop object in a particular mode.

func CFRunLoopStop(CFRunLoop!)

Forces a CFRunLoop object to stop running.

func CFRunLoopIsWaiting(CFRunLoop!) -> Bool

Returns a Boolean value that indicates whether the run loop is waiting for an event.

