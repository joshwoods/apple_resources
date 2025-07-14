

- Kernel
- IOKit Fundamentals
- Workflow and Control
-  IOEventSource 

Class

# IOEventSource

Abstract class for all work-loop event sources.

macOS 10.0+

``` source
class IOEventSource : OSObject
```

## Overview

The IOEventSource declares the abstract super class that all event sources must inherit from if an IOWorkLoop is to receive events from them.

An event source can represent any event that should cause the work-loop of a device to wake up and perform work. Two examples of event sources are the IOInterruptEventSource which delivers interrupt notifications and IOCommandGate which delivers command requests.

A kernel module can always use the work-loop model for serialising access to anything at all. The IOEventSource is used for communicating events to the work-loop, and the chain of event sources should be used to walk the possible event sources and demultipex them. Note a particular instance of an event source may only be a member of 1 linked list chain. If you need to move it between chains than make sure it is removed from the original chain before attempting to move it.

The IOEventSource makes no attempt to maintain the consistency of its internal data across multi-threading. It is assumed that the user of these basic tools will protect the data that these objects represent in some sort of device wide instance lock. For example the IOWorkLoop maintains the event chain by using an IOCommandGate and thus single threading access to its state.

All subclasses of IOEventSource that wish to perform work on the work-loop thread are expected to implement the checkForWork() member function. As of macOS, 10.7 (Darwin 11), checkForWork is no longer pure virtual, and should not be overridden if there is no work to be done.

checkForWork() is the key method in this class. It is called by some work-loop when convienient and is expected to evaluate its internal state and determine if an event has occurred since the last call. In the case of an event having occurred then the instance defined target(owner)/action will be called. The action is stored as an ordinary C function pointer but the first parameter is always the owner. This means that a C++ member function can be used as an action function though this depends on the ABI.

Although the eventChainNext variable contains a reference to the next event source in the chain this reference is not retained. The list 'owner' i.e. the client that creates the event, not the work-loop, is expected to retain the source.

## Topics

### Miscellaneous

checkForWork

Virtual member function used by IOWorkLoop for work scheduling.

disable

Disable event source.

enable

Enable event source.

getAction

Get'ter for \$link action variable.

getNext

Get'ter for \$link eventChainNext variable.

getWorkLoop

Get'ter for \$link workLoop variable.

init

Primary initialiser for the IOEventSource class.

isEnabled

Get'ter for \$link enable variable.

onThread

Convenience function for workLoop-\>onThread.

setAction

Set'ter for \$link action variable.

setNext

Set'ter for \$link eventChainNext variable.

setWorkLoop

Set'ter for \$link workLoop variable.

### Callbacks

Action

### Constants

Miscellaneous Defines

### DataTypes

ExpansionData

### Instance Variables

workLoop

reserved

refcon

owner

eventChainNext

enabled

action

### Instance Methods

- checkForWork

- closeGate

- disable

- enable

- free

- getAction

- getActionBlock

- getMetaClass

- getNext

- getRefcon

- getWorkLoop

- init

- isEnabled

- onThread

- openGate

- setAction

- setActionBlock

- setNext

- setRefcon

- setWorkLoop

- signalWorkAvailable

- sleepGate

- sleepGate

- tryCloseGate

- wakeupGate

## Relationships

### Inherits From

- OSObject

## See Also

### Base Types

IOCommandPool

Manipulates a pool of commands which inherit from IOCommand.

IOCommandGate

Single-threaded work-loop client request mechanism.

IOCommand

This class is an abstract class which represents an I/O command.

IODispatchSource

