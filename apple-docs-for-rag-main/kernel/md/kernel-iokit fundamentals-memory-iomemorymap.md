

- Kernel
- IOKit Fundamentals
- Memory
-  IOMemoryMap 

Class

# IOMemoryMap

A class defining common methods for describing a memory mapping.

macOS 10.0+

``` source
class IOMemoryMap : OSObject
```

## Overview

The IOMemoryMap object represents a mapped range of memory, described by a IOMemoryDescriptor. The mapping may be in the kernel or a non-kernel task and has processor cache mode attributes. IOMemoryMap instances are created by IOMemoryDescriptor when it creates mappings in its map method, and returned to the caller.

## Topics

### Miscellaneous

getAddress()

Accessor to the length of the mapping.

getAddressTask

Accessor to the task of the mapping.

getLength

Accessor to the length of the mapping.

getMapOptions

Accessor to the options the mapping was created with.

getMemoryDescriptor

Accessor to the IOMemoryDescriptor the mapping was created from.

getPhysicalAddress

Return the physical address of the first byte in the mapping.

getPhysicalSegment

Break a mapping into its physically contiguous segments.

getSize()

Accessor to the length of the mapping.

getVirtualAddress

Accessor to the virtual address of the first byte in the mapping.

redirect

Replace the memory mapped in a process with new backing memory.

unmap

Force the IOMemoryMap to unmap, without destroying the object.

### Instance Methods

- getAddress

- getSize

- Dispatch

- GetAddress

Returns the address of the memory block.

- GetLength

Returns the length of the memory block in bytes.

- GetOffset

Returns the offset from the original start of the memory block.

- free

Performs any final cleanup for the memory map object.

- getAddressTask

- getLength

- getMapOptions

- getMemoryDescriptor

- getMetaClass

- getPhysicalAddress

- getPhysicalSegment

- getVirtualAddress

- redirect

- taggedRelease

- taskDied

- unmap

- wireRange

## Relationships

### Inherits From

- OSObject

## See Also

### Mapped Memory

IOMapper

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

