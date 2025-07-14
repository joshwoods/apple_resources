

- DriverKit
- IODataQueueDispatchSource
-  DataAvailable 

Instance Method

# DataAvailable

Responds to the addition of new data to the queue.

DriverKitiOSiPadOSmacOS

``` source
void DataAvailable(OSAction * action);
```

## Parameters 

`action`  

The action object being executed.

## Mentioned in 

Creating a Driver Using the DriverKit SDK

## Discussion

Use this method as a prototype for declaring your own custom data-queue handlers. When declaring your method, use the TYPE macro to indicate that your method has the same parameters and return value as this method.

Use the implementation of your method to examine the data in the queue and remove it when appropriate.

## See Also

### Removing Work from the Queue

SetDataAvailableHandler

Sets the handler block to run when another object adds data to the queue.

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

