

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOWorkLoop
-  free 

# free

``` source
virtual void free(); 
```

## Overview

Mandatory free of the object independent of the current retain count. If the work loop is running, this method will not return until the thread has successfully terminated. Each event source in the chain will be released and the working semaphore will be destroyed.

If the client has some outstanding requests on an event they will never be informed of completion. If an external thread is blocked on any of the event sources they will be awakened with a KERN_INTERUPTED status.

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

