

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOCommandGate
-  runCommand 

# runCommand

Single thread a command with the target work-loop.

``` source
virtual IOReturn runCommand(
 void *arg0 = 0,
 void *arg1 = 0, 
 void *arg2 = 0,
 void *arg3 = 0); 
```

## Parameters 

`arg0`  

Parameter for action of command gate, defaults to 0.

`arg1`  

Parameter for action of command gate, defaults to 0.

`arg2`  

Parameter for action of command gate, defaults to 0.

`arg3`  

Parameter for action of command gate, defaults to 0.

## Return Value

kIOReturnSuccess if successful. kIOReturnAborted if a disabled command gate is free()ed before being reenabled, kIOReturnNoResources if no action available.

## Overview

Client function that causes the current action to be called in a single threaded manner. Beware the work-loop's gate is recursive and command gates can cause direct or indirect re-entrancy. When the executing on a client's thread runCommand will sleep until the work-loop's gate opens for execution of client actions, the action is single threaded against all other work-loop event sources. If the command is disabled the attempt to run a command will be stalled until enable is called.

## See Also

### Miscellaneous

attemptAction

Single thread a call to an action with the target work-loop.

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

