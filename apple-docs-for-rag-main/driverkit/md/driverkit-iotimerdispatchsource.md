

- DriverKit
-  IOTimerDispatchSource 

Class

# IOTimerDispatchSource

A dispatch source that notifies your driver at a specific time.

DriverKitiOSiPadOSmacOS

``` source
class IOTimerDispatchSource;
```

## Overview

An IOTimerDispatchSource object executes an associated action at a designated time. After configuring the dispatch source object, call the WakeAtTime method to schedule the time at which to execute your code. There are several timebases you can use to configure the timer, but the most common one is kIOTimerClockMachAbsoluteTime.

## Topics

### Configuring the Timer Source

Create

Creates and configures a timer dispatch object.

init

Handles the basic initialization of the dispatch source.

free

Performs any final cleanup for the timer dispatch source.

SetHandler

Sets the handler block to run when the timer fires.

### Rescheduling the Timer

WakeAtTime

Schedules a callback from the timer.

Clock Types

Clock types to use when configuring a timer.

### Starting and Stopping the Timer Source

SetEnableWithCompletion

Enables or disables the timer.

Cancel

Cancels all callbacks from the event source.

### Declaring Actions

TimerOccurred

Executes custom code when the timer fires.

CheckForWork

Checks for events to handle.

## Relationships

### Inherits From

- IODispatchSource

## See Also

### Event management

IODispatchQueue

An object that manages the serial execution of blocks.

IOInterruptDispatchSource

A dispatch source that reports hardware-related interrupt events to your driver.

IODataQueueDispatchSource

A dispatch source that manages a shared-memory data queue.

IODispatchSource

The common base class for dispatch sources.

OSAction

An object that executes your driver’s custom behavior.

