

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOCommandGate
-  commandWakeup 

# commandWakeup

Wakeup one or more threads that are asleep on an event.

``` source
virtual void commandWakeup(
 void *event,
 bool oneThread = false); 
```

## Parameters 

`event`  

Pointer to an address.

`onlyOneThread`  

true to only wake up at most one thread, false otherwise.

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

