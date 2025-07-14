

- DriverKit
- IODataQueueDispatchSource
-  Enqueue 

Instance Method

# Enqueue

Adds a single entry to the shared data queue.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t Enqueue(uint32_t dataSize, IODataQueueClientEnqueueEntryBlockcallback);
```

## Parameters 

`dataSize`  

The size of the data to enqueue.

`callback`  

The callback to execute when there is enough space to enqueue the data.

## Return Value

kIOReturnSuccess on success, kIOReturnOverrun if the queue was full, or kIOReturnError if the queue is corrupt. See Error Codes.

## See Also

### Adding Work to the Queue

SetDataServicedHandler

Installs the handler block to execute when data is removed from the queue.

DataServiced

Responds to the removal of data from the queue.

EnqueueWithCoalesce

Adds an entry to the queue, but doesn’t automatically send a data-available notification.

SendDataAvailable

Sends a notification to observers that indicates more data is available for processing.

IODataQueueClientEnqueueEntryBlock

The handler block you use to add data to a queue.

