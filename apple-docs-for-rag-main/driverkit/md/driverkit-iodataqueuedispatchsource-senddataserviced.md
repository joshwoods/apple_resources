

- DriverKit
- IODataQueueDispatchSource
-  SendDataServiced 

Instance Method

# SendDataServiced

Notifies interested parties that you removed data from the queue.

DriverKitiOSiPadOSmacOS

``` source
void SendDataServiced();
```

## Discussion

Use this method to send a single notification after dequeueing multiple entries with the DequeueWithCoalesce method. The DequeueWithCoalesce method doesn’t call the DataServiced handler automatically after removing an entry. Instead, you call this method after the successful removal of entries from the queue.

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

IODataQueueClientDequeueEntryBlock

The handler block you use to remove data from a queue.

