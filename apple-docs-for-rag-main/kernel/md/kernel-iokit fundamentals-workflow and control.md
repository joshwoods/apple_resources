

- Kernel
- IOKit Fundamentals
-  Workflow and Control 

API Collection

# Workflow and Control

## Topics

### Work Loops

IOWorkLoop

### Timers

IOTimerEventSource

Time based event source mechanism.

IOWatchDogTimer

IOGetTimeDeprecated

IOTimeStampConstant

IOTimeStampEndConstant

IOTimeStampStartConstant

### Sleep

IODelay

Spin delay for a number of microseconds.

IOPause

Spin delay for a number of nanoseconds.

IOSleep

Sleep the calling thread for a number of milliseconds.

IOSleepWithLeeway

### Dispatch Queues

IODispatchQueueInterface

IODispatchSourceInterface

IODispatchQueue

### Data Queues

IODataQueueDispatchSource

IODataQueueDispatchSourceInterface

IODataQueue

A generic queue designed to pass data from the kernel to a user process.

### Output Queues

IOGatedOutputQueue

An extension of an IOBasicOutputQueue.

IOBasicOutputQueue

A concrete implementation of an IOOutputQueue.

IOOutputQueue

A packet queue that supports multiple producers and a single consumer.

### Notifications

IOServiceNotificationDispatchSource

IOServiceNotificationDispatchSourceInterface

IONotifier

An abstract base class defining common methods for controlling a notification request.

### Interrupts

IOInterruptDispatchSource

IOInterruptDispatchSourceInterface

IOFilterInterruptEventSource

Filtering varient of the \$link IOInterruptEventSource.

IOInterruptEventSource

Event source for interrupt delivery to work-loop based drivers.

IOInterruptController

PassthruInterruptController

IOInterruptSource

IOInterruptVector

### Base Types

IOCommandPool

Manipulates a pool of commands which inherit from IOCommand.

IOCommandGate

Single-threaded work-loop client request mechanism.

IOCommand

This class is an abstract class which represents an I/O command.

IODispatchSource

IOEventSource

Abstract class for all work-loop event sources.

## See Also

### Resources

Memory

Allocate, map, free, and manage memory in the kernel.

Locks

Data Types

Create strings, numbers, collections, data objects, and the other standard types employed by drivers and kernel extensions.

