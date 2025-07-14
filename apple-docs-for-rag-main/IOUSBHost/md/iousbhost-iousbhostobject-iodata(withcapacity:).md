

- IOUSBHost
- IOUSBHostObject
-  ioData(withCapacity:) 

Instance Method

# ioData(withCapacity:)

Allocates a buffer for input/output requests.

Mac Catalyst 14.0+macOS 10.15+

``` source
func ioData(withCapacity capacity: Int) throws -> NSMutableData
```

## Parameters 

`capacity`  

The size, in bytes, of the buffer to allocate.

## Return Value

A pointer to an allocated buffer.

## Discussion

This method allocates and maps a kernel buffer that the underlying controller hardware has optimized. Using this method, the buffer doesn’t bounce to perform DMA operations.

Important

Because the kernel backs the NSMutableData object, the length and capacity aren’t mutable. Any changes to the length or capacity throws an exception.

