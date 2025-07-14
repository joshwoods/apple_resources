

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOTimerEventSource
-  enable 

# enable

Enables a call to the action.

``` source
virtual void enable(); 
```

## Overview

Allows the action function to be called. If the timer event source was disabled while a call was outstanding and the call wasn't cancelled then it will be rescheduled. So a disable/enable pair will disable calls from this event source.

## See Also

### Miscellaneous

cancelTimeout

Disable any outstanding calls to this event source.

disable

Disable a timed callout.

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

