

- Kernel
- IOKit Fundamentals
- Workflow and Control
-  IODispatchQueue 

Class

# IODispatchQueue

macOS 10.15+

``` source
class IODispatchQueue : OSObject, IODispatchQueueInterface
```

## Topics

### Instance Methods

- Cancel

Stops the queue from dequeueing any further tasks, and notifies the specified handler when all in-flight tasks finish.

- Dispatch

- DispatchAsync

Schedule a block for asynchronous execution on the current queue.

- DispatchAsync_f

Schedule a C-style function for asynchrous execution on the current queue.

- DispatchConcurrent

- DispatchConcurrent_f

- DispatchSync

Schedule a block for synchronous execution on the current queue.

- DispatchSync_f

Schedule a C-style function for synchronous execution on the current queue.

- GetName

Returns the name of the queue as a C string.

- OnQueue

Returns a Boolean value that indicates whether the current thread matches the dispatch queue's thread.

- RunAction

- SetPort

- SetPort_Impl

- Sleep

- SleepWithDeadline

- SleepWithTimeout

- Wakeup

- WakeupWithOptions

- free

Performs any final cleanup for the dispatch queue object.

- getMetaClass

- init

Initializes the dispatch queue object.

### Type Methods

+ Create

Creates a new dispatch queue object.

+ Create_Call

+ Create_Impl

+ Create_Invoke

+ Log

Log the current execution context with respect to any queues the current thread holds.

+ SetPort_Invoke

## Relationships

### Inherits From

- IODispatchQueueInterface
- OSObject

## See Also

### Dispatch Queues

IODispatchQueueInterface

IODispatchSourceInterface

