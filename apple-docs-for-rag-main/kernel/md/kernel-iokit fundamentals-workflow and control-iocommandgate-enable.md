

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOCommandGate
-  enable 

# enable

Enable command gate, this will unblock any blocked Commands and Actions.

``` source
virtual void enable(); 
```

## Overview

Enable the command gate. The attemptAction/attemptCommand calls will now be enabled and can succeeed. Stalled runCommand/runAction calls will be woken up.

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

init

Class initialiser.

runAction

Single thread a call to an action with the target work-loop.

runCommand

Single thread a command with the target work-loop.

