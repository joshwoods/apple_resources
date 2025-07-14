

- Kernel
- IOKit Fundamentals
- Memory
- IOBufferMemoryDescriptor
-  Dispatch 

Instance Method

# Dispatch

macOS 10.15+

``` source
virtual kern_return_t Dispatch(const IORPC rpc);
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

- SetLength_Impl

