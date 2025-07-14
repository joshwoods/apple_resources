

- Kernel
- IOKit Fundamentals
- Memory
-  IOMapper 

Class

# IOMapper

macOS 10.2+

``` source
class IOMapper : IOService
```

## Topics

### Creating a Mapper Object

+ copyMapperForDevice

+ copyMapperForDeviceWithIndex

- initHardware

- start

- free

### Mapping Memory Addresses

- mapToPhysicalAddress

- iovmMapMemory

- iovmUnmapMemory

- iovmInsert

### Determining the Mapper's Availability

+ checkForSystemMapper

+ setMapperRequired

+ waitForSystemMapper

### Getting Configuration Details

- getMetaClass

- getPageSize

## Relationships

### Inherits From

- IOService

## See Also

### Mapped Memory

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

IOFlushProcessorCache

Flushes the processor cache for mapped memory.

