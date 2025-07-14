

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOCommandGate
-  attemptAction 

# attemptAction

Single thread a call to an action with the target work-loop.

``` source
virtual IOReturn attemptAction(
 Action action, 
 void *arg0 = 0,
 void *arg1 = 0, 
 void *arg2 = 0,
 void *arg3 = 0); 
```

## Parameters 

`action`  

Pointer to function to be executed in work-loop context.

`arg0`  

Parameter for action parameter, defaults to 0.

`arg1`  

Parameter for action parameter, defaults to 0.

`arg2`  

Parameter for action parameter, defaults to 0.

`arg3`  

Parameter for action parameter, defaults to 0.

## Return Value

kIOReturnSuccess if successful. kIOReturnBadArgument if action is not defined, kIOReturnNotPermitted if this event source is currently disabled, kIOReturnCannotLock if lock attempt fails.

## Overview

Client function that causes the given action to be called in a single threaded manner. Beware the work-loop's gate is recursive and command gates can cause direct or indirect re-entrancy. When the executing on a client's thread attemptCommand will fail if the work-loop's gate is closed.

## See Also

### Miscellaneous

attemptCommand

Single thread a command with the target work-loop.

commandGate

Factory method to create and initialise an IOCommandGate, See \$link init.

commandSleep(void *, AbsoluteTime, UInt32)

Put a thread that is currently holding the command gate to sleep.

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

