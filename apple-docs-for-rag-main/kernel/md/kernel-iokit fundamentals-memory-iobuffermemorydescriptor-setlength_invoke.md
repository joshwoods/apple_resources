

- Kernel
- IOKit Fundamentals
- Memory
- IOBufferMemoryDescriptor
-  SetLength_Invoke 

Type Method

# SetLength_Invoke

macOS 10.15+

``` source
static kern_return_t SetLength_Invoke(const IORPC rpc, OSMetaClassBase *target, SetLength_Handler func);
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

- SetLength

Changes the length of the memory buffer.

- SetLength_Impl

- Dispatch

