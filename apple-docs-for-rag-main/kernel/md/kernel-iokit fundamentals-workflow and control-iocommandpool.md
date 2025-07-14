

- Kernel
- IOKit Fundamentals
- Workflow and Control
-  IOCommandPool 

Class

# IOCommandPool

Manipulates a pool of commands which inherit from IOCommand.

DriverKitKernelDriverKit 21.0+macOS 10.6+

``` source
class IOCommandPool : OSObject
```

## Overview

The IOCommandPool class is used to manipulate a pool of commands which inherit from IOCommand. It includes a factory method to create a pool of a certain size. Once the factory method is invoked, the semaphore is set to zero. The caller must then put commands in the pool by creating the command (via the controller's factory method or a memory allocation) and calling the returnCommand method with the newly created command as its argument.

## Topics

### Miscellaneous

commandPool

Should never be used, obsolete. See IOCommandPool::withWorkLoop.

gatedGetCommand

gatedReturnCommand

getCommand

init

Should never be used, obsolete. See initWithWorkLoop.

initWithWorkLoop

Primary initializer for an IOCommandPool object.

returnCommand

withWorkLoop(IOService *, IOWorkLoop *, UInt32)

Should never be used, obsolete. See IOCommandPool::withWorkLoop.

withWorkLoop(IOWorkLoop *)

Primary factory method for the IOCommandPool class

### Constants

kIOCommandPoolDefaultSize

The default size of any command pool.

### DataTypes

ExpansionData

### Instance Variables

reserved

### Instance Methods

- free

- gatedGetCommand

- gatedReturnCommand

- getCommand

- getMetaClass

- init

- init

- initWithQueue

- initWithWorkLoop

- returnCommand

### Type Methods

+ commandPool

+ withQueue

+ withWorkLoop

## Relationships

### Inherits From

- OSObject
- OSObject

## See Also

### Base Types

IOCommandGate

Single-threaded work-loop client request mechanism.

IOCommand

This class is an abstract class which represents an I/O command.

IODispatchSource

IOEventSource

Abstract class for all work-loop event sources.

