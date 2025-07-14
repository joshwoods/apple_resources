

- Kernel
- IOKit Fundamentals
- Memory
-  IOFlushProcessorCache 

Function

# IOFlushProcessorCache

Flushes the processor cache for mapped memory.

macOS 10.0+

``` source
IOReturn IOFlushProcessorCache(task_t task, IOVirtualAddress address, IOByteCount length);
```

## Parameters 

`task`  

Task the memory is mapped into.

`address`  

Virtual address of the memory.

`length`  

Length of the range to set.

## Return Value

An IOReturn code.

## Discussion

This function flushes the processor cache of an already mapped memory range. Note in most cases it is preferable to use IOMemoryDescriptor::prepare and complete to manage cache coherency since they are aware of the architecture's requirements. Flushing the processor cache is not required for coherency in most situations.

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

IOMapperInsertPage

