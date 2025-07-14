

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOWorkLoop
-  removeEventSource 

# removeEventSource

``` source
virtual IOReturn removeEventSource(
 IOEventSource *toRemove); 
```

## Parameters 

`toRemove`  

Pointer to IOEventSource subclass to remove.

## Return Value

Returns kIOReturnSuccess if successful, kIOReturnBadArgument if toRemove couldn't be found.

## Overview

Remove an event source from the work loop. This function does not return until the work loop has acknowledged the removal of the event source. When an event has been removed the threadMain will always restart its loop and check all outstanding events. The event source will be released before return.

## See Also

### Miscellaneous

_maintRequest

Synchronous implementation of addEventSource and removeEventSource functions.

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

