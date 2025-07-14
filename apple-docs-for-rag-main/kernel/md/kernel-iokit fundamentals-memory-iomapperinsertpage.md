

- Kernel
- IOKit Fundamentals
- Memory
-  IOMapperInsertPage 

Function

# IOMapperInsertPage

macOS 10.2+

``` source
ppnum_t IOMapperInsertPage(ppnum_t addr, unsigned int offset, ppnum_t page);
```

## See Also

### Mapped Memory

IOMapper

IOMemoryMap

A class defining common methods for describing a memory mapping.

IOMappedRead16

Read two bytes from the desired "Physical" IOSpace address.

IOMappedRead32

Read four bytes from the desired "Physical" IOSpace address.

IOMappedRead64

Read eight bytes from the desired "Physical" IOSpace address.

IOMappedRead8

Read one byte from the desired "Physical" IOSpace address.

IOMappedWrite16

Write two bytes to the desired "Physical" IOSpace address.

IOMappedWrite32

Write four bytes to the desired "Physical" IOSpace address.

IOMappedWrite64

Write eight bytes to the desired "Physical" IOSpace address.

IOMappedWrite8

Write one byte to the desired "Physical" IOSpace address.

IOMapperIOVMAlloc

IOMapperIOVMFree

IOFlushProcessorCache

Flushes the processor cache for mapped memory.

