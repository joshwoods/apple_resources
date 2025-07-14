

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOWorkLoop
-  runEventSources 

# runEventSources

``` source
virtual bool runEventSources(); 
```

## Return Value

Return false if the work loop is shutting down, true otherwise.

## Overview

Consists of the inner 2 loops of the threadMain function(qv). The outer loop terminates when there is no more work, and the inside loop walks the event list calling the checkForWork method in each event source. If an event source has more work to do, it can set the more flag and the outer loop will repeat.

This function can be used to clear a priority inversion between the normal workloop thread and multimedia's real time threads. The problem is that the interrupt action routine is often held off by high priority threads. So if they want to get their data now they will have to call us and ask if any data is available. The multi-media user client will arrange for this function to be called, which causes any pending interrupts to be processed and the completion routines called. By the time the function returns all outstanding work will have been completed at the real time threads priority.

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

threadMain

threadMainContinuation

Static function that calls the threadMain function.

workLoop

Factory member function to construct and intialize a work loop.

workLoopWithOptions

Factory member function to constuct and intialize a work loop.

workLoopWithOptions(IOOptionBits options)

Factory member function to constuct and intialize a work loop.

