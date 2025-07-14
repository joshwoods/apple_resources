

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOCommandGate
-  commandGate 

# commandGate

Factory method to create and initialise an IOCommandGate, See \$link init.

``` source
static IOCommandGate *commandGate(
 OSObject *owner,
 Action action = 0); 
```

## Return Value

Returns a pointer to the new command gate if sucessful, 0 otherwise.

## See Also

### Miscellaneous

attemptAction

Single thread a call to an action with the target work-loop.

attemptCommand

Single thread a command with the target work-loop.

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

