

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOTimerEventSource
-  wakeAtTime(AbsoluteTime) 

# wakeAtTime(AbsoluteTime)

Setup a callback at this absolute time.

``` source
virtual IOReturn wakeAtTime(
 AbsoluteTimeabstime); 
```

## Parameters 

`abstime`  

Absolute Time when to wake up, counted in 'decrementer' units and starts at zero when system boots.

## Return Value

kIOReturnSuccess if everything is fine, kIOReturnNoResources if action hasn't been declared by init or IOEventSource::setAction (qqv).

## Overview

Starts the timer, which will expire at abstime. After it expires, the timer will call the 'action' registered in the init() function. This timer is not periodic, a further call is needed to reset and restart the timer after it expires.

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

setTimeout(UInt32, UInt32)

Setup a callback at after the delay in some unit. See wakeAtTime(AbsoluteTime).

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

wakeAtTime(UInt32, UInt32)

Setup a callback at this absolute time. See wakeAtTime(AbsoluteTime).

wakeAtTimeMS

Setup a callback at this absolute time. See wakeAtTime(AbsoluteTime).

wakeAtTimeTicks

Setup a callback at this absolute time. See wakeAtTime(AbsoluteTime).

wakeAtTimeUS

Setup a callback at this absolute time. See wakeAtTime(AbsoluteTime).

