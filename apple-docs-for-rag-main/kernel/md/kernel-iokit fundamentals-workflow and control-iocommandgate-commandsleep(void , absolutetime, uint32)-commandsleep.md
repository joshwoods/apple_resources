

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOCommandGate
-  commandSleep(void \*, AbsoluteTime, UInt32) 

# commandSleep(void \*, AbsoluteTime, UInt32)

Put a thread that is currently holding the command gate to sleep.

``` source
virtual IOReturn commandSleep(
 void *event, 
 AbsoluteTimedeadline, 
 UInt32interruptible); 
```

## Parameters 

`event`  

Pointer to an address.

`deadline`  

Clock deadline to timeout the sleep.

`interruptible`  

THREAD_UNINT, THREAD_INTERRUPTIBLE or THREAD_ABORTSAFE. THREAD_UNINT specifies that the sleep cannot be interrupted by a signal. THREAD_INTERRUPTIBLE specifies that the sleep may be interrupted by a "kill -9" signal. THREAD_ABORTSAFE specifies that the sleep may be interrupted by any user signal.

## Return Value

THREAD_AWAKENED - normal wakeup, THREAD_TIMED_OUT - timeout expired, THREAD_INTERRUPTED - interrupted, THREAD_RESTART - restart operation entirely, kIOReturnNotPermitted if the calling thread does not hold the command gate.

## Overview

Put a thread to sleep waiting for an event but release the gate first. If the event occurs or timeout occurs then the commandGate is closed before the function returns.

## See Also

### Miscellaneous

attemptAction

Single thread a call to an action with the target work-loop.

attemptCommand

Single thread a command with the target work-loop.

commandGate

Factory method to create and initialise an IOCommandGate, See \$link init.

commandSleep(void *, UInt32)

Put a thread that is currently holding the command gate to sleep.

commandWakeup

Wakeup one or more threads that are asleep on an event.

disable

Disable the command gate

enable

Enable command gate, this will unblock any blocked Commands and Actions.

init

Class initialiser.

runAction

Single thread a call to an action with the target work-loop.

runCommand

Single thread a command with the target work-loop.

