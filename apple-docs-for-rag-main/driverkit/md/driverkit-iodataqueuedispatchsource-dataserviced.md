

- DriverKit
- IODataQueueDispatchSource
-  DataServiced 

Instance Method

# DataServiced

Responds to the removal of data from the queue.

DriverKitiOSiPadOSmacOS

``` source
void DataServiced(OSAction * action);
```

## Parameters 

`action`  

The action object being executed.

## Discussion

Use this method as a prototype for declaring your own custom data-queue handler. When declaring your method, use the TYPE macro to indicate that your method has the same parameters and return value as this method.

Use the implementation of your method to add more data to the queue or perform other relevant tasks.

## See Also

### Adding Work to the Queue

SetDataServicedHandler

Installs the handler block to execute when data is removed from the queue.

Enqueue

Adds a single entry to the shared data queue.

EnqueueWithCoalesce

Adds an entry to the queue, but doesn’t automatically send a data-available notification.

SendDataAvailable

Sends a notification to observers that indicates more data is available for processing.

IODataQueueClientEnqueueEntryBlock

The handler block you use to add data to a queue.

