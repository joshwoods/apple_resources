

- DriverKit
- IODataQueueDispatchSource
-  SetDataServicedHandler 

Instance Method

# SetDataServicedHandler

Installs the handler block to execute when data is removed from the queue.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t SetDataServicedHandler(OSAction * action);
```

## Parameters 

`action`  

The OSAction object that contains the callback method to execute. The data queue retains your action object until you install a new handler or cancel the dispatch source. The system executes your callback on the dispatch queue you designated in your OSAction object.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

If your code produces data for the queue, use this method to install a handler so you can add more data to the queue. When space becomes available in the queue, the system executes your handler.

## See Also

### Adding Work to the Queue

DataServiced

Responds to the removal of data from the queue.

Enqueue

Adds a single entry to the shared data queue.

EnqueueWithCoalesce

Adds an entry to the queue, but doesn’t automatically send a data-available notification.

SendDataAvailable

Sends a notification to observers that indicates more data is available for processing.

IODataQueueClientEnqueueEntryBlock

The handler block you use to add data to a queue.

