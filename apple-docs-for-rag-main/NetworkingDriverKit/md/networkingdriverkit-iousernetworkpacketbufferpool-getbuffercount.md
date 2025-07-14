

- NetworkingDriverKit
- IOUserNetworkPacketBufferPool
-  GetBufferCount 

Instance Method

# GetBufferCount

Returns the number of buffers associated with the network packet buffer pool.

DriverKit

``` source
kern_return_t GetBufferCount(uint32_t * count);
```

## Parameters 

`count`  

On output, the number of buffers in the pool. It is a programmer error to specify `NULL` or an invalid pointer for this parameter.

## Return Value

`kIOReturnSuccess` on success, or another value if an error occurred.

## See Also

### Getting Pool Information

GetPacketCount

Returns the number of network packets that the pool is capable of storing.

