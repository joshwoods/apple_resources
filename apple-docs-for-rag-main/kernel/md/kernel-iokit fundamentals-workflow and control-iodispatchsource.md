

- Kernel
- IOKit Fundamentals
- Workflow and Control
-  IODispatchSource 

Class

# IODispatchSource

macOS 10.15+

``` source
class IODispatchSource : OSObject, IODispatchSourceInterface
```

## Topics

### Instance Methods

- Cancel

- CheckForWork

- Dispatch

- SetEnable

- SetEnableWithCompletion

- SetEnable_Impl

- free

Performs any final cleanup for the dispatch source.

- getMetaClass

- init

Handles the basic initialization of the dispatch source.

### Type Methods

+ Cancel_Invoke

+ CheckForWork_Invoke

+ SetEnableWithCompletion_Invoke

+ SetEnable_Invoke

## Relationships

### Inherits From

- IODispatchSourceInterface
- OSObject

## See Also

### Base Types

IOCommandPool

Manipulates a pool of commands which inherit from IOCommand.

IOCommandGate

Single-threaded work-loop client request mechanism.

IOCommand

This class is an abstract class which represents an I/O command.

IOEventSource

Abstract class for all work-loop event sources.

