

- DriverKit
- IODataQueueDispatchSource
-  SetDataAvailableHandler 

Instance Method

# SetDataAvailableHandler

Sets the handler block to run when another object adds data to the queue.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t SetDataAvailableHandler(OSAction * action);
```

## Parameters 

`action`  

The OSAction instance specifying the callback method. The data queue retains this object until you call this method again or call Cancel. This queue executes the action’s handler method on the action’s own dispatch queue.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## See Also

### Removing Work from the Queue

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

