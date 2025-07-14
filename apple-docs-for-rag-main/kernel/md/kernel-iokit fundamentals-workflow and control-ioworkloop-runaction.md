

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOWorkLoop
-  runAction 

# runAction

Single thread a call to an action with the work-loop.

``` source
virtual IOReturn runAction(
 Action action,
 OSObject *target, 
 void *arg0 = 0,
 void *arg1 = 0, 
 void *arg2 = 0,
 void *arg3 = 0); 
```

## Parameters 

`action`  

Pointer to function to be executed in work-loop context.

`arg0`  

Parameter for action parameter, defaults to 0.

`arg1`  

Parameter for action parameter, defaults to 0.

`arg2`  

Parameter for action parameter, defaults to 0.

`arg3`  

Parameter for action parameter, defaults to 0.

## Return Value

Returns the value of the Action callout.

## Overview

Client function that causes the given action to be called in a single threaded manner. Beware: the work-loop's gate is recursive and runAction can cause direct or indirect re-entrancy. When executing on a client's thread, runAction will sleep until the work-loop's gate opens for execution of client actions, the action is single threaded against all other work-loop event sources.

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

