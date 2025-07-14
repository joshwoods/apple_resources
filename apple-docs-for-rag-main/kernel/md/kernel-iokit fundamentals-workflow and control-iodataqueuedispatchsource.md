

- Kernel
- IOKit Fundamentals
- Workflow and Control
-  IODataQueueDispatchSource 

Class

# IODataQueueDispatchSource

macOS 10.15+

``` source
class IODataQueueDispatchSource : IODispatchSource, IODataQueueDispatchSourceInterface
```

## Topics

### Instance Methods

- CanEnqueueData

- CanEnqueueData

- Cancel_Impl

- CheckForWork_Impl

- CopyDataAvailableHandler

- CopyDataAvailableHandler_Impl

- CopyDataServicedHandler

- CopyDataServicedHandler_Impl

- CopyMemory

- CopyMemory_Impl

- DataAvailable

- DataServiced

- Dequeue

Removes the next entry from the queue.

- DequeueWithCoalesce

Removes the next queue entry, but doesn't automatically send notifications.

- Dispatch

- Enqueue

Adds a single entry to the shared data queue.

- EnqueueWithCoalesce

Adds an entry to the queue, but doesn't automatically send a data-available notification.

- IsDataAvailable

Checks whether the data queue contains data to process.

- Peek

Returns the next queue entry without removing it from the queue.

- SendDataAvailable

Sends a notification to observers that indicates more data is available for processing.

- SendDataServiced

Notifies interested parties that you removed data from the queue.

- SetDataAvailableHandler

- SetDataAvailableHandler_Impl

- SetDataServicedHandler

- SetDataServicedHandler_Impl

- SetEnableWithCompletion_Impl

- free

Performs any final cleanup for the data-queue dispatch source.

- getMetaClass

- init

Handles the basic initialization of the dispatch source.

### Type Methods

+ CopyDataAvailableHandler_Invoke

+ CopyDataServicedHandler_Invoke

+ CopyMemory_Invoke

+ Create

Creates a dispatch source that you use as a shared-memory data queue.

+ Create_Impl

+ Create_Invoke

+ DataAvailable_Invoke

+ DataAvailable_Invoke

+ DataServiced_Invoke

+ DataServiced_Invoke

+ GetDataQueueEntryHeaderSize

+ SetDataAvailableHandler_Invoke

+ SetDataServicedHandler_Invoke

## Relationships

### Inherits From

- IODataQueueDispatchSourceInterface
- IODispatchSource

## See Also

### Data Queues

IODataQueueDispatchSourceInterface

IODataQueue

A generic queue designed to pass data from the kernel to a user process.

