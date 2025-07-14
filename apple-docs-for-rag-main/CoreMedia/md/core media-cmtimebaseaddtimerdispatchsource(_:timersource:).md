

- Core Media
-  CMTimebaseAddTimerDispatchSource(\_:timerSource:) 

Function

# CMTimebaseAddTimerDispatchSource(\_:timerSource:)

Adds the timer dispatch source to the list of timers the timebase manages.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMTimebaseAddTimerDispatchSource(
    _ timebase: CMTimebase,
    timerSource: dispatch_source_t
) -> OSStatus
```

## Discussion

You must create the timer source by calling `dispatch_source_create(DISPATCH_SOURCE_TYPE_TIMER, 0, 0, some_dispatch_queue)` and associate an event handler with it from `dispatch_source_set_event_handler(timerSource, some_handler_block)` or `dispatch_source_set_event_handler_f(timerSource, some_handler_function)`. Call `dispatch_resume(timerSource)` because the system creates dispatch sources in a suspended state.

The timebase retains the timer source, and maintains its start time according to the `CMTime` set using CMTimebaseSetTimerDispatchSourceNextFireTime(_:timerSource:fireTime:flags:). Until the first call to CMTimebaseSetTimerDispatchSourceNextFireTime(_:timerSource:fireTime:flags:), the system sets the start time to `DISPATCH_TIME_FOREVER`.

For more information on dispatch sources, see Dispatch Sources.

## See Also

### Interacting with Timers

func CMTimebaseAddTimer(CMTimebase, timer: CFRunLoopTimer, runloop: CFRunLoop) -> OSStatus

Adds the timer to the list of timers the timebase manages.

func CMTimebaseRemoveTimer(CMTimebase, timer: CFRunLoopTimer) -> OSStatus

Removes the timer from the list of timers the timebase manages.

func CMTimebaseRemoveTimerDispatchSource(CMTimebase, timerSource: dispatch_source_t) -> OSStatus

Removes the timer dispatch source from the list of timers the timebase manages.

func CMTimebaseSetTimerNextFireTime(CMTimebase, timer: CFRunLoopTimer, fireTime: CMTime, flags: UInt32) -> OSStatus

Sets the time on the timebase’s timeline at which the timer should fire next.

func CMTimebaseSetTimerToFireImmediately(CMTimebase, timer: CFRunLoopTimer) -> OSStatus

Sets the timer to fire immediately once, overriding any previous timer calls.

func CMTimebaseSetTimerDispatchSourceNextFireTime(CMTimebase, timerSource: dispatch_source_t, fireTime: CMTime, flags: UInt32) -> OSStatus

Sets the time on the timebase’s timeline at which the timer dispatch source should fire next.

func CMTimebaseSetTimerDispatchSourceToFireImmediately(CMTimebase, timerSource: dispatch_source_t) -> OSStatus

Sets the timer dispatch source to fire immediately once, overriding any previous timer call.

