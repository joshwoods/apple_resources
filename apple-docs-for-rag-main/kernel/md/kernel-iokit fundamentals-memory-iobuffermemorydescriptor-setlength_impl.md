

- Kernel
- IOKit Fundamentals
- Memory
- IOBufferMemoryDescriptor
-  SetLength_Impl 

Instance Method

# SetLength_Impl

macOS 10.15+

``` source
kern_return_t SetLength_Impl(uint64_t length);
```

## See Also

### Managing Internal Structures

ExpansionData

reserved

+ Create

Creates a new memory buffer descriptor object in the current process space.

+ Create_Impl

+ Create_Invoke

- GetAddressRange

Returns the address and length of the memory buffer.

- getMetaClass

+ SetLength_Invoke

- SetLength

Changes the length of the memory buffer.

- Dispatch

