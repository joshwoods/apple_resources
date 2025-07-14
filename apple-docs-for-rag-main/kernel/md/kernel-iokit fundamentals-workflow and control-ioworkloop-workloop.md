

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOWorkLoop
-  workLoop 

# workLoop

Factory member function to construct and intialize a work loop.

``` source
static IOWorkLoop *workLoop(); 
```

## Return Value

Returns a workLoop instance if constructed successfully, 0 otherwise.

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

threadMain

threadMainContinuation

Static function that calls the threadMain function.

workLoopWithOptions

Factory member function to constuct and intialize a work loop.

workLoopWithOptions(IOOptionBits options)

Factory member function to constuct and intialize a work loop.

