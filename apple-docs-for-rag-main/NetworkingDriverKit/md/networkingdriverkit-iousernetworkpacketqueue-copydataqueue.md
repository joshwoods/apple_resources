

- NetworkingDriverKit
- IOUserNetworkPacketQueue
-  CopyDataQueue 

Instance Method

# CopyDataQueue

Returns the dispatch queue that this object uses to execute tasks.

DriverKit

``` source
kern_return_t CopyDataQueue(IODataQueueDispatchSource * * dataQueue);
```

## Parameters 

`dataQueue`  

On return, a pointer to the dispatch source that this object uses to generate tasks.

## Return Value

`kIOReturnSuccess` on success, or another value if an error occurred.

## See Also

### Managing the Data Queue

SetDataQueue

Assigns the specified dispatch source to this object.

