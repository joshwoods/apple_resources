

- USBDriverKit
- IOUSBHostPipe
-  CreateMemoryDescriptorRing 

Instance Method

# CreateMemoryDescriptorRing

DriverKit 19.0+

``` source
kern_return_t CreateMemoryDescriptorRing(uint32_t size);
```

## Parameters 

`size`  

Size of the ring.

## Return Value

KERN_SUCCESS is successful see IOReturn.h for error codes.

## Discussion

The ring must only be created once, and will be freed by the kernel driver when the pipe is destroyed.

