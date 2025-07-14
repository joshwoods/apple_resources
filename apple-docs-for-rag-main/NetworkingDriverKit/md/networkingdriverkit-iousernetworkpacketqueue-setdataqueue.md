

- NetworkingDriverKit
- IOUserNetworkPacketQueue
-  SetDataQueue 

Instance Method

# SetDataQueue

Assigns the specified dispatch source to this object.

DriverKit

``` source
kern_return_t SetDataQueue(IODataQueueDispatchSource * dataQueue);
```

## Parameters 

`dataQueue`  

The new data queue to use when executing tasks.

## Return Value

`kIOReturnSuccess` on success, or another value if an error occurred.

## Discussion

Use this method to change the dispatch queue that this object uses to perform tasks. This method releases the previous dispatch queue, if any, and retains the new object in the `dataQueue` parameter.

## See Also

### Managing the Data Queue

CopyDataQueue

Returns the dispatch queue that this object uses to execute tasks.

