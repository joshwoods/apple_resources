

- Kernel
- IOKit Fundamentals
- Workflow and Control
-  IOTimerEventSource 

Class

# IOTimerEventSource

Time based event source mechanism.

macOS 10.0+

``` source
class IOTimerEventSource : IOEventSource
```

## Overview

An event source that implements a simple timer. A timeout handler is called once the timeout period expires. This timeout handler will be called by the work-loop that this event source is attached to.

Usually a timer event source will be used to implement a timeout. In general when a driver makes a request it will need to setup a call to keep track of when the I/O doesn't complete. This class is designed to make that somewhat easier.

Remember the system doesn't guarantee the accuracy of the callout. It is possible that a higher priority thread is running which will delay the execution of the action routine. In fact the thread will be made runable at the exact requested time, within the accuracy of the CPU's decrementer based interrupt, but the scheduler will then control execution.

## Topics

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

### Callbacks

Action

### DataTypes

ExpansionData

### Instance Variables

reserved

calloutEntry

abstime

### Instance Methods

- cancelTimeout

- checkForWork

- disable

- enable

- free

- getMetaClass

- init

- init

- setTimeout

- setTimeout

- setTimeout

- setTimeoutFunc

- setTimeoutMS

- setTimeoutTicks

- setTimeoutUS

- setWorkLoop

- wakeAtTime

- wakeAtTime

- wakeAtTime

- wakeAtTimeMS

- wakeAtTimeTicks

- wakeAtTimeUS

### Type Methods

+ timeout

+ timeoutAndRelease

+ timeoutSignaled

+ timerEventSource

+ timerEventSource

+ timerEventSource

## Relationships

### Inherits From

- IOEventSource

## See Also

### Timers

IOWatchDogTimer

IOGetTimeDeprecated

IOTimeStampConstant

IOTimeStampEndConstant

IOTimeStampStartConstant

