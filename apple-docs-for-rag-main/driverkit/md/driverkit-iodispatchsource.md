

- DriverKit
-  IODispatchSource 

Class

# IODispatchSource

The common base class for dispatch sources.

DriverKitiOSiPadOSmacOS

``` source
class IODispatchSource;
```

## Topics

### Configuring the Dispatch Source

init

Handles the basic initialization of the dispatch source.

free

Performs any final cleanup for the dispatch source.

Cancel

Cancel all callbacks from the dispatch source.

### Enabling and Disabling the Source

SetEnable

Enables or disables the delivery of events to your code.

SetEnableWithCompletion

Enables or disables the dispatch source.

### Checking the State of the Source

CheckForWork

Checks for events to handle.

## Relationships

### Inherits From

- OSObject

### Inherited By

- IODataQueueDispatchSource
- IOInterruptDispatchSource
- IOServiceNotificationDispatchSource
- IOServiceStateNotificationDispatchSource
- IOTimerDispatchSource

## See Also

### Event management

IODispatchQueue

An object that manages the serial execution of blocks.

IOInterruptDispatchSource

A dispatch source that reports hardware-related interrupt events to your driver.

IOTimerDispatchSource

A dispatch source that notifies your driver at a specific time.

IODataQueueDispatchSource

A dispatch source that manages a shared-memory data queue.

OSAction

An object that executes your driver’s custom behavior.

