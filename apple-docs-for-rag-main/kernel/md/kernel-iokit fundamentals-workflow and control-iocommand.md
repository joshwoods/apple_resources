

- Kernel
- IOKit Fundamentals
- Workflow and Control
-  IOCommand 

Class

# IOCommand

This class is an abstract class which represents an I/O command.

DriverKitKernelDriverKit 21.0+macOS 10.6+

``` source
class IOCommand : OSObject
```

## Overview

This class is an abstract class which represents an I/O command passed from a device driver to a controller. All controller commands (e.g. IOATACommand) should inherit from this class.

## Topics

### Instance Variables

fCommandChain

### Instance Methods

- CommandChain

- free

- getMetaClass

- init

### Type Methods

+ FromChain

## Relationships

### Inherits From

- OSObject
- OSObject

## See Also

### Base Types

IOCommandPool

Manipulates a pool of commands which inherit from IOCommand.

IOCommandGate

Single-threaded work-loop client request mechanism.

IODispatchSource

IOEventSource

Abstract class for all work-loop event sources.

