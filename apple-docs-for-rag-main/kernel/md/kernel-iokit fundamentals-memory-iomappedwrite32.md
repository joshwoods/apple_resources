

- Kernel
- IOKit Fundamentals
- Memory
-  IOMappedWrite32 

Function

# IOMappedWrite32

Write four bytes to the desired "Physical" IOSpace address.

macOS 10.2+

``` source
void IOMappedWrite32(IOPhysicalAddress address, UInt32 value);
```

## Parameters 

`address`  

The desired address, as returned by IOMemoryDescriptor::getPhysicalSegment.

`value`  

Data to be writen to the desired location

## Discussion

Write four bytes to the desired "Physical" IOSpace address. This function allows the developer to write to an address returned from any memory descriptor's getPhysicalSegment routine.

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

IOMappedWrite64

Write eight bytes to the desired "Physical" IOSpace address.

IOMappedWrite8

Write one byte to the desired "Physical" IOSpace address.

IOMapperIOVMAlloc

IOMapperIOVMFree

IOMapperInsertPage

IOFlushProcessorCache

Flushes the processor cache for mapped memory.

