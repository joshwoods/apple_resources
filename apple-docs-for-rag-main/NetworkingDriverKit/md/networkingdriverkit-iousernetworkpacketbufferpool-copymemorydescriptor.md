

- NetworkingDriverKit
- IOUserNetworkPacketBufferPool
-  CopyMemoryDescriptor 

Instance Method

# CopyMemoryDescriptor

Returns a memory descriptor for the buffer pool’s contents.

DriverKit

``` source
kern_return_t CopyMemoryDescriptor(IOMemoryDescriptor * * memory);
```

## Parameters 

`memory`  

On output, a pointer to a memory descriptor object. It is a programmer error to specify `NULL` or an invalid pointer for this parameter.

## Return Value

`kIOReturnSuccess` on success, or another value if an error occurred.

