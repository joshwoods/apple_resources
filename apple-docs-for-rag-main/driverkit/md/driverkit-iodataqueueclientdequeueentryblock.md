

- DriverKit
-  IODataQueueClientDequeueEntryBlock 

Type Alias

# IODataQueueClientDequeueEntryBlock

The handler block you use to remove data from a queue.

DriverKitiOSiPadOSmacOS

``` source
typedef void (^)(const void *, unsigned long) IODataQueueClientDequeueEntryBlock;
```

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

DequeueWithCoalesce

Removes the next queue entry, but doesn’t automatically send notifications.

SendDataServiced

Notifies interested parties that you removed data from the queue.

