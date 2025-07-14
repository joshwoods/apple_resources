

- DriverKit
- IODataQueueDispatchSource
-  SendDataAvailable 

Instance Method

# SendDataAvailable

Sends a notification to observers that indicates more data is available for processing.

DriverKitiOSiPadOSmacOS

``` source
void SendDataAvailable();
```

## See Also

### Adding Work to the Queue

SetDataServicedHandler

Installs the handler block to execute when data is removed from the queue.

DataServiced

Responds to the removal of data from the queue.

Enqueue

Adds a single entry to the shared data queue.

EnqueueWithCoalesce

Adds an entry to the queue, but doesn’t automatically send a data-available notification.

IODataQueueClientEnqueueEntryBlock

The handler block you use to add data to a queue.

