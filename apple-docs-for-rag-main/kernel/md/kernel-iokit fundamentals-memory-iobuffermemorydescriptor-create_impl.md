

- Kernel
- IOKit Fundamentals
- Memory
- IOBufferMemoryDescriptor
-  Create_Impl 

Type Method

# Create_Impl

macOS 10.15+

``` source
static kern_return_t Create_Impl(uint64_t options, uint64_t capacity, uint64_t alignment, IOBufferMemoryDescriptor **memory);
```

## See Also

### Managing Internal Structures

ExpansionData

reserved

+ Create

Creates a new memory buffer descriptor object in the current process space.

+ Create_Invoke

- GetAddressRange

Returns the address and length of the memory buffer.

- getMetaClass

+ SetLength_Invoke

- SetLength

Changes the length of the memory buffer.

- SetLength_Impl

- Dispatch

