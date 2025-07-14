

- USBDriverKit
- IOUSBHostInterface
-  CreateIOBuffer 

Instance Method

# CreateIOBuffer

Allocates a buffer for use during I/O operations.

DriverKit 19.0+

``` source
kern_return_t CreateIOBuffer(IOOptionBits options, uint64_t capacity, IOBufferMemoryDescriptor * * buffer);
```

## Parameters 

`options`  

The direction of I/O transfer for the buffer. For a list of possible values, see `Memory Buffer Options`.

`capacity`  

The size of the buffer to allocate in bytes.

`buffer`  

A pointer to a variable. On success, this variable contains a pointer to a memory descriptor. It’s your responsibility to release this memory descriptor when you finish using it. If an error occurs, the method returns NULL instead.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

This method allocates an IOBufferMemoryDescriptor optimized for use by the underlying controller hardware. A buffer allocated by this method isn’t bounced to perform DMA operations.

