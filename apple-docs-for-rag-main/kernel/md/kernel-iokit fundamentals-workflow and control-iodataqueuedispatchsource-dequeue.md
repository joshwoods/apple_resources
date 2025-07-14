

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IODataQueueDispatchSource
-  Dequeue 

Instance Method

# Dequeue

Removes the next entry from the queue.

DriverKitKernelDriverKit 19.0+macOS 10.15.2+

``` source
kern_return_t Dequeue(IODataQueueClientDequeueEntryBlock callback);
```

## Parameters 

`callback`  

The callback you use to process the next entry in the queue.

## Return Value

kIOReturnSuccess on success, kIOReturnUnderrun if the queue is empty, or kIOReturnError if the queue is corrupt. See `Error Codes`.

## See Also

### Removing Work from the Queue

- SetDataAvailableHandler

Sets the handler block to run when another object adds data to the queue.

- DataAvailable

Responds to the addition of new data to the queue.

IODataQueueClientDequeueEntryBlock

The handler block you use to remove data from a queue.

- IsDataAvailable

Checks whether the data queue contains data to process.

- Peek

Returns the next queue entry without removing it from the queue.

- DequeueWithCoalesce

Removes the next queue entry, but doesn't automatically send notifications.

- SendDataServiced

Notifies interested parties that you removed data from the queue.

