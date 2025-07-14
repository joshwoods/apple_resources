

- Core Media
-  CMTimebaseRemoveTimerDispatchSource(\_:timerSource:) 

Function

# CMTimebaseRemoveTimerDispatchSource(\_:timerSource:)

Removes the timer dispatch source from the list of timers the timebase manages.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimebaseRemoveTimerDispatchSource(
    _ timebase: CMTimebase,
    timerSource: dispatch_source_t
) -> OSStatus
```

## Discussion

The timebase no longer maintains the timer source’s start time. If the system cancels the timer source, the timebase eventually removes it from its list and releases it even if you don’t call this function.

## See Also

### Interacting with Timers

func CMTimebaseAddTimer(CMTimebase, timer: CFRunLoopTimer, runloop: CFRunLoop) -> OSStatus

Adds the timer to the list of timers the timebase manages.

func CMTimebaseAddTimerDispatchSource(CMTimebase, timerSource: dispatch_source_t) -> OSStatus

Adds the timer dispatch source to the list of timers the timebase manages.

func CMTimebaseRemoveTimer(CMTimebase, timer: CFRunLoopTimer) -> OSStatus

Removes the timer from the list of timers the timebase manages.

func CMTimebaseSetTimerNextFireTime(CMTimebase, timer: CFRunLoopTimer, fireTime: CMTime, flags: UInt32) -> OSStatus

Sets the time on the timebase’s timeline at which the timer should fire next.

func CMTimebaseSetTimerToFireImmediately(CMTimebase, timer: CFRunLoopTimer) -> OSStatus

Sets the timer to fire immediately once, overriding any previous timer calls.

func CMTimebaseSetTimerDispatchSourceNextFireTime(CMTimebase, timerSource: dispatch_source_t, fireTime: CMTime, flags: UInt32) -> OSStatus

Sets the time on the timebase’s timeline at which the timer dispatch source should fire next.

func CMTimebaseSetTimerDispatchSourceToFireImmediately(CMTimebase, timerSource: dispatch_source_t) -> OSStatus

Sets the timer dispatch source to fire immediately once, overriding any previous timer call.

