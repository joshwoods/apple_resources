

- DriverKit
- IODataQueueDispatchSource
-  DequeueWithCoalesce 

Instance Method

# DequeueWithCoalesce

Removes the next queue entry, but doesn’t automatically send notifications.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t DequeueWithCoalesce(bool * sendDataServiced, IODataQueueClientDequeueEntryBlockcallback);
```

## Parameters 

`sendDataServiced`  

A Boolean value that indicates that this method would have sent a notification. Initialize the value to `false`, and then make one or more calls to this method. If the value is `true` after all of those calls, call the SendDataServiced method yourself to deliver the notification.

`callback`  

The callback that you use to process the dequeued data.

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

Peek

Returns the next queue entry without removing it from the queue.

Dequeue

Removes the next entry from the queue.

SendDataServiced

Notifies interested parties that you removed data from the queue.

IODataQueueClientDequeueEntryBlock

The handler block you use to remove data from a queue.

