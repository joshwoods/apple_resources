

- Kernel
- IOKit Fundamentals
- Workflow and Control
-  IOWorkLoop 

Class

# IOWorkLoop

macOS 10.0+

``` source
class IOWorkLoop : OSObject
```

## Overview

An IOWorkLoop is a thread of control that is intended to be used to provide single threaded access to hardware. This class has no knowledge of the nature and type of the events that it marshals and forwards. When a device driver successfully starts (see IOService::start), it is expected to create the event sources it will need to receive events. Then a work loop is initialized and the events are added to the work loop for monitoring. In general this set up will be automated by the family superclass of the specific device.

The thread main method walks the event source linked list and messages each one requesting a work check. At this point each event source is expected to notify its registered owner that the event has occurred. After each event has been walked and each indicates that another loop isn't required (by setting the 'more' flag to false) the thread will go to sleep on a signaling semaphore.

When an event source is registered with a work loop it is informed of the semaphore to use to wake up the loop.

## Topics

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

workLoop

Factory member function to construct and intialize a work loop.

workLoopWithOptions

Factory member function to constuct and intialize a work loop.

workLoopWithOptions(IOOptionBits options)

Factory member function to constuct and intialize a work loop.

### Callbacks

Action

### DataTypes

maintCommandEnum

ExpansionData

### Instance Variables

workToDoLock

workToDo

workThread

reserved

loopRestart

gateLock

eventChain

controlG

### Instance Methods

- addEventSource

- closeGate

- disableAllEventSources

- disableAllInterrupts

- enableAllEventSources

- enableAllInterrupts

- eventSourcePerformsWork

- free

- getMetaClass

- getThread

- inGate

- init

- onThread

- openGate

- removeEventSource

- runAction

- runActionBlock

- runEventSources

- setMaximumLockTime

- signalWorkAvailable

- sleepGate

- sleepGate

- threadMain

- tryCloseGate

- wakeupGate

### Type Methods

+ releaseEventChain

+ threadMainContinuation

+ workLoop

+ workLoopWithOptions

## Relationships

### Inherits From

- OSObject

