

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOWorkLoop
-  \_maintRequest 

# \_maintRequest

Synchronous implementation of addEventSource and removeEventSource functions.

``` source
virtual IOReturn _maintRequest(
 void *command,
 void *data,
 void *,
 void *); 
```

## Return Value

kIOReturnUnsupported if the command given is not implemented, kIOReturnSuccess otherwise.

## Overview

This function implements the commands as defined in the maintCommandEnum. It can be subclassed but it isn't an external API in the usual sense. A subclass implementation of \_maintRequest would be called synchronously with respect to the work loop and it should be implemented in the usual way that an ioctl would be.

## See Also

### Miscellaneous

addEventSource

disableAllEventSources

Calls disable() in all event sources.

disableAllInterrupts

Calls disable() in all interrupt event sources.

enableAllEventSources

Calls enable() in all event sources.

enableAllInterrupts

Calls enable() in all interrupt event sources.

eventSourcePerformsWork

Checks if the event source passed in overrides checkForWork() to perform any work. IOWorkLoop uses this to determine if the event source should be polled in runEventSources() or not.

free

getThread

Gets the workThread.

inGate

Is the current execution context holding the work-loop's gate?

init

onThread

Is the current execution context on the work thread?

removeEventSource

runAction

Single thread a call to an action with the work-loop.

runEventSources

threadMain

threadMainContinuation

Static function that calls the threadMain function.

workLoop

Factory member function to construct and intialize a work loop.

workLoopWithOptions

Factory member function to constuct and intialize a work loop.

workLoopWithOptions(IOOptionBits options)

Factory member function to constuct and intialize a work loop.

