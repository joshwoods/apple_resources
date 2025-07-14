

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOTimerEventSource
-  setTimeout(UInt32, UInt32) 

# setTimeout(UInt32, UInt32)

Setup a callback at after the delay in some unit. See wakeAtTime(AbsoluteTime).

``` source
virtual IOReturn setTimeout(
 UInt32interval, 
 UInt32 scale_factor = scale_factor); 
```

## Parameters 

`interval`  

Delay from now to wake up in some defined unit.

`scale_factor`  

Define the unit of interval, default to nanoseconds.

## Return Value

kIOReturnSuccess if everything is fine, kIOReturnNoResources if action hasn't been declared.

## See Also

### Miscellaneous

cancelTimeout

Disable any outstanding calls to this event source.

disable

Disable a timed callout.

enable

Enables a call to the action.

free

Sub-class implementation of free method, frees calloutEntry

init

Initializes the timer with an owner, and a handler to call when the timeout expires.

setTimeout(AbsoluteTime)

Setup a callback at after the delay in decrementer ticks. See wakeAtTime(AbsoluteTime).

setTimeoutFunc

Set's timeout as the function of calloutEntry.

setTimeoutMS

Setup a callback at after the delay in milliseconds. See wakeAtTime(AbsoluteTime).

setTimeoutTicks

Setup a callback at after the delay in scheduler ticks. See wakeAtTime(AbsoluteTime).

setTimeoutUS

Setup a callback at after the delay in microseconds. See wakeAtTime(AbsoluteTime).

timeout

Function that routes the call from the OS' timeout mechanism into a work-loop context.

timerEventSource

Allocates and returns an initialized timer instance.

wakeAtTime(AbsoluteTime)

Setup a callback at this absolute time.

wakeAtTime(UInt32, UInt32)

Setup a callback at this absolute time. See wakeAtTime(AbsoluteTime).

wakeAtTimeMS

Setup a callback at this absolute time. See wakeAtTime(AbsoluteTime).

wakeAtTimeTicks

Setup a callback at this absolute time. See wakeAtTime(AbsoluteTime).

wakeAtTimeUS

Setup a callback at this absolute time. See wakeAtTime(AbsoluteTime).

