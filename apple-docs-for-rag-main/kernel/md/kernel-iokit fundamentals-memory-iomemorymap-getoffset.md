

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryMap
-  GetOffset 

Instance Method

# GetOffset

Returns the offset from the original start of the memory block.

DriverKitKernelDriverKit 19.0+macOS 10.15.2+

``` source
uint64_t GetOffset(void);
```

## Return Value

The number of bytes from the start of the original block of memory to the first byte of this memory map object.

## Discussion

When creating a memory map object, you can map to a location in the middle of the underlying buffer. You might do this to access a specific structure inside that buffer. This method returns the offset from the original start of the buffer to the first byte of your mapping.

## See Also

### Getting the Map Attributes

- GetAddress

Returns the address of the memory block.

- GetLength

Returns the length of the memory block in bytes.

