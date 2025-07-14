

- Kernel
- IOKit Fundamentals
- Memory
- IOBufferMemoryDescriptor
-  Create_Invoke 

Type Method

# Create_Invoke

macOS 10.15+

``` source
static kern_return_t Create_Invoke(const IORPC rpc, Create_Handler func);
```

## See Also

### Managing Internal Structures

ExpansionData

reserved

+ Create

Creates a new memory buffer descriptor object in the current process space.

+ Create_Impl

- GetAddressRange

Returns the address and length of the memory buffer.

- getMetaClass

+ SetLength_Invoke

- SetLength

Changes the length of the memory buffer.

- SetLength_Impl

- Dispatch

