

- Kernel
- IOKit Fundamentals
- Memory
-  IOMappedRead16 

Function

# IOMappedRead16

Read two bytes from the desired "Physical" IOSpace address.

macOS 10.2+

``` source
UInt16 IOMappedRead16(IOPhysicalAddress address);
```

## Parameters 

`address`  

The desired address, as returned by IOMemoryDescriptor::getPhysicalSegment.

## Return Value

Data contained at that location

## Discussion

Read two bytes from the desired "Physical" IOSpace address. This function allows the developer to read an address returned from any memory descriptor's getPhysicalSegment routine. It can then be used by segmenting a physical page slightly to tag the physical page with its kernel space virtual address.

## See Also

### Mapped Memory

IOMapper

IOMemoryMap

A class defining common methods for describing a memory mapping.

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

IOFlushProcessorCache

Flushes the processor cache for mapped memory.

