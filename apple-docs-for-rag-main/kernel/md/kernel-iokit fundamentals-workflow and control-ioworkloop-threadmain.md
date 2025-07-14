

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOWorkLoop
-  threadMain 

# threadMain

``` source
virtual void threadMain(); 
```

## Overview

Work loop threads main function. This function consists of 3 loops: the outermost loop is the semaphore clear and wait loop, the middle loop terminates when there is no more work, and the inside loop walks the event list calling the checkForWork method in each event source. If an event source has more work to do, it can set the more flag and the middle loop will repeat. When no more work is outstanding the outermost will sleep until an event is signalled.

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

removeEventSource

runAction

Single thread a call to an action with the work-loop.

runEventSources

threadMainContinuation

Static function that calls the threadMain function.

workLoop

Factory member function to construct and intialize a work loop.

workLoopWithOptions

Factory member function to constuct and intialize a work loop.

workLoopWithOptions(IOOptionBits options)

Factory member function to constuct and intialize a work loop.

