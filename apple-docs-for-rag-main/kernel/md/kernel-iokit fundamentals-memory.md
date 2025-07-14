

- Kernel
- IOKit Fundamentals
-  Memory 

API Collection

# Memory

Allocate, map, free, and manage memory in the kernel.

## Topics

### Descriptors

IOBufferMemoryDescriptor

A simple memory descriptor that allocates its own buffer memory.

IODeviceMemory

An IOMemoryDescriptor used for device physical memory ranges.

IOGeneralMemoryDescriptor

IOInterleavedMemoryDescriptor

The IOInterleavedMemoryDescriptor object describes a memory area made up of portions of several other IOMemoryDescriptors.

IOMultiMemoryDescriptor

The IOMultiMemoryDescriptor object describes a memory area made up of several other IOMemoryDescriptors.

IOSubMemoryDescriptor

The IOSubMemoryDescriptor object describes a memory area made up of a portion of another IOMemoryDescriptor.

IOMemoryDescriptor

An abstract base class that defines common methods for describing physical or virtual memory.

### Direct Memory Access (DMA)

IODMACommand

An object that converts memory references to I/O bus addresses.

IODMAController

IODMAEventSource

### Deallocation

IOFree

Frees memory allocated with IOMalloc.

IOFreeAligned

Frees memory allocated with IOMallocAligned.

IOFreePageable

Frees memory allocated with IOMallocPageable.

### Allocation

IOMalloc

Allocates general purpose, wired memory in the kernel map.

IOMallocAligned

Allocates wired memory in the kernel map, with an alignment restriction.

IOMallocPageable

Allocates pageable memory in the kernel map.

IOMallocZero

IORangeAllocator

A utility class to manage allocations from a range.

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

IOFlushProcessorCache

Flushes the processor cache for mapped memory.

### Cursors

IOBigMemoryCursor

An IOMemoryCursor subclass that outputs a vector of PhysicalSegments in the big endian byte order.

IOLittleMemoryCursor

An IOMemoryCursor subclass that outputs a vector of PhysicalSegments in the little endian byte order.

IONaturalMemoryCursor

An IOMemoryCursor subclass that outputs a vector of PhysicalSegments in the natural byte orientation for the CPU.

IOMemoryCursor

A mechanism to convert memory references to physical addresses.

## See Also

### Resources

Workflow and Control

Locks

Data Types

Create strings, numbers, collections, data objects, and the other standard types employed by drivers and kernel extensions.

