

- DriverKit
- IODataQueueDispatchSource
-  Peek 

Instance Method

# Peek

Returns the next queue entry without removing it from the queue.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t Peek(IODataQueueClientDequeueEntryBlockcallback);
```

## Parameters 

`callback`  

The callback you use to examine the next entry in the queue.

## Return Value

kIOReturnSuccess on success, kIOReturnUnderrun if the queue is empty, or kIOReturnError if the queue is corrupt. See Error Codes.

## See Also

### Removing Work from the Queue

SetDataAvailableHandler

Sets the handler block to run when another object adds data to the queue.

DataAvailable

Responds to the addition of new data to the queue.

IsDataAvailable

Checks whether the data queue contains data to process.

Dequeue

Removes the next entry from the queue.

DequeueWithCoalesce

Removes the next queue entry, but doesn’t automatically send notifications.

SendDataServiced

Notifies interested parties that you removed data from the queue.

IODataQueueClientDequeueEntryBlock

The handler block you use to remove data from a queue.

