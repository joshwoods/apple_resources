

- DriverKit
- IODataQueueDispatchSource
-  EnqueueWithCoalesce 

Instance Method

# EnqueueWithCoalesce

Adds an entry to the queue, but doesn’t automatically send a data-available notification.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t EnqueueWithCoalesce(uint32_t dataSize, bool * sendDataAvailable, IODataQueueClientEnqueueEntryBlockcallback);
```

## Parameters 

`dataSize`  

The size of the data to enqueue.

`sendDataAvailable`  

A Boolean value that indicates that this method would have sent a notification. Initialize the value to `false`, and then make one or more calls to this method. If the value is `true` after all of those calls, call the SendDataAvailable method yourself to deliver the notification.

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

Enqueue

Adds a single entry to the shared data queue.

SendDataAvailable

Sends a notification to observers that indicates more data is available for processing.

IODataQueueClientEnqueueEntryBlock

The handler block you use to add data to a queue.

