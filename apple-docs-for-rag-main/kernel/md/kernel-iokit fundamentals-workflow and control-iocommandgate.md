

- Kernel
- IOKit Fundamentals
- Workflow and Control
-  IOCommandGate 

Class

# IOCommandGate

Single-threaded work-loop client request mechanism.

macOS 10.0+

``` source
class IOCommandGate : IOEventSource
```

## Overview

An IOCommandGate instance is an extremely lightweight mechanism that executes an action on the driver's work-loop. 'On the work-loop' is actually a lie but the work-loop single threaded semantic is maintained for this event source. Using the work-loop gate rather than execution by the workloop. The command gate tests for a potential self dead lock by checking if the runCommand request is made from the work-loop's thread, it doesn't check for a mutual dead lock though where a pair of work loop's dead lock each other.

The IOCommandGate is a lighter weight version of the IOCommandQueue and should be used in preference. Generally use a command queue whenever you need a client to submit a request to a work loop. A typical command gate action would check if the hardware is active, if so it will add the request to a pending queue internal to the device or the device's family. Otherwise if the hardware is inactive then this request can be acted upon immediately.

CAUTION: The runAction, runCommand, and attemptCommand functions cannot be called from an interrupt context.

## Topics

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

init

Class initialiser.

runAction

Single thread a call to an action with the target work-loop.

runCommand

Single thread a command with the target work-loop.

### Callbacks

Action

### DataTypes

ExpansionData

### Instance Variables

reserved

### Instance Methods

- attemptAction

- attemptCommand

- commandSleep

- commandSleep

- commandWakeup

- disable

- enable

- free

- getMetaClass

- init

- runAction

- runActionBlock

- runCommand

- setWorkLoop

### Type Methods

+ commandGate

## Relationships

### Inherits From

- IOEventSource

## See Also

### Base Types

IOCommandPool

Manipulates a pool of commands which inherit from IOCommand.

IOCommand

This class is an abstract class which represents an I/O command.

IODispatchSource

IOEventSource

Abstract class for all work-loop event sources.

