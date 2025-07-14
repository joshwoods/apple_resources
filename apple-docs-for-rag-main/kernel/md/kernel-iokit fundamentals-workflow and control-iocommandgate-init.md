

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOCommandGate
-  init 

# init

Class initialiser.

``` source
virtual bool init(
 OSObject *owner,
 Action action = 0); 
```

## Parameters 

`owner`  

Owner of this, newly created, instance of the IOCommandGate. This argument will be used as the first parameter in the action callout.

`action`  

Pointer to a C function that is called whenever a client of the IOCommandGate calls runCommand. NB Can be a C++ member function but caller must cast the member function to \$link IOCommandGate::Action and they will get a compiler warning. Defaults to zero, see \$link IOEventSource::setAction.

## Return Value

True if inherited classes initialise successfully.

## Overview

Initialiser for IOCommandGate operates only on newly 'newed' objects. Shouldn't be used to re-init an existing instance.

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

runAction

Single thread a call to an action with the target work-loop.

runCommand

Single thread a command with the target work-loop.

