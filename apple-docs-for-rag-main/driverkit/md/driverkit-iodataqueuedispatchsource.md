

- DriverKit
-  IODataQueueDispatchSource 

Class

# IODataQueueDispatchSource

A dispatch source that manages a shared-memory data queue.

DriverKitiOSiPadOSmacOS

``` source
class IODataQueueDispatchSource;
```

## Mentioned in 

Creating a Driver Using the DriverKit SDK

## Topics

### Configuring the Dispatch Source

Create

Creates a dispatch source that you use as a shared-memory data queue.

init

Handles the basic initialization of the dispatch source.

free

Performs any final cleanup for the data-queue dispatch source.

### Adding Work to the Queue

SetDataServicedHandler

Installs the handler block to execute when data is removed from the queue.

DataServiced

Responds to the removal of data from the queue.

Enqueue

Adds a single entry to the shared data queue.

EnqueueWithCoalesce

Adds an entry to the queue, but doesn’t automatically send a data-available notification.

SendDataAvailable

Sends a notification to observers that indicates more data is available for processing.

IODataQueueClientEnqueueEntryBlock

The handler block you use to add data to a queue.

### Removing Work from the Queue

SetDataAvailableHandler

Sets the handler block to run when another object adds data to the queue.

DataAvailable

Responds to the addition of new data to the queue.

IsDataAvailable

Checks whether the data queue contains data to process.

Peek

Returns the next queue entry without removing it from the queue.

Dequeue

Removes the next entry from the queue.

DequeueWithCoalesce

Removes the next queue entry, but doesn’t automatically send notifications.

SendDataServiced

Notifies interested parties that you removed data from the queue.

IODataQueueClientDequeueEntryBlock

The handler block you use to remove data from a queue.

### Starting and Stopping the Dispatch Source

SetEnableWithCompletion

Controls the enable state of the interrupt source.

Cancel

Cancels all callbacks from the dispatch source.

### Performing Internal Tasks

CopyDataAvailableHandler

A private method that the dispatch source uses to detect enqueued data.

CopyDataServicedHandler

A private method that the dispatch source uses to detect dequeued data.

CopyMemory

A private method that the dispatch source uses to copy memory.

CheckForWork

Checks for events to handle.

### Instance Methods

CanEnqueueData

CanEnqueueData

### Type Methods

GetDataQueueEntryHeaderSize

## Relationships

### Inherits From

- IODispatchSource

## See Also

### Event management

IODispatchQueue

An object that manages the serial execution of blocks.

IOInterruptDispatchSource

A dispatch source that reports hardware-related interrupt events to your driver.

IOTimerDispatchSource

A dispatch source that notifies your driver at a specific time.

IODispatchSource

The common base class for dispatch sources.

OSAction

An object that executes your driver’s custom behavior.

