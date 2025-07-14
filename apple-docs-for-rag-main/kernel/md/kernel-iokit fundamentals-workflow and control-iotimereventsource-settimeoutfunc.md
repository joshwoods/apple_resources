

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOTimerEventSource
-  setTimeoutFunc 

# setTimeoutFunc

Set's timeout as the function of calloutEntry.

``` source
virtual void setTimeoutFunc(); 
```

## Overview

IOTimerEventSource is based upon the kern/thread_call.h APIs currently. This function allocates the calloutEntry member variable by using thread_call_allocate(timeout, this). If you need to write your own subclass of IOTimerEventSource you probably should override this method to allocate an entry that points to your own timeout routine.

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

