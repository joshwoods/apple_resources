

- NetworkingDriverKit
- IOUserNetworkPacketQueue
-  SetPacketBufferPool 

Instance Method

# SetPacketBufferPool

Assigns the specified buffer pool with this queue.

DriverKit

``` source
kern_return_t SetPacketBufferPool(IOUserNetworkPacketBufferPool * pool);
```

## Parameters 

`pool`  

The new buffer pool to associate with the queue.

## Return Value

`kIOReturnSuccess` on success, or another value if an error occurred.

## Discussion

Use this method to change the buffer pool that provides network packets to the queue. This method releases the previous pool, if any, and retains the new object in the `pool` parameter.

## See Also

### Configuring the Queue Attributes

SetPacketDirection

Specifies whether packets flow into or out of the queue.

