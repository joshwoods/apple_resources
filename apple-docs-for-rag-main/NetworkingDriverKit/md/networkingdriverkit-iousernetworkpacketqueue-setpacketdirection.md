

- NetworkingDriverKit
- IOUserNetworkPacketQueue
-  SetPacketDirection 

Instance Method

# SetPacketDirection

Specifies whether packets flow into or out of the queue.

DriverKit

``` source
kern_return_t SetPacketDirection(IOUserNetworkPacketDirection direction);
```

## Parameters 

`direction`  

The direction for network packets to travel.

## Return Value

`kIOReturnSuccess` on success, or another value if an error occurred.

## Discussion

Typically, you do not call this method yourself. The concrete subclasses set the direction during initialization.

## See Also

### Configuring the Queue Attributes

SetPacketBufferPool

Assigns the specified buffer pool with this queue.

