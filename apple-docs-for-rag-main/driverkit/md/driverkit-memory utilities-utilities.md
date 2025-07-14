

- DriverKit
-  Memory Utilities 

API Collection

# Memory Utilities

Allocate and deallocate memory and manage memory pointers in different address spaces.

## Topics

### Allocation

IONew

Allocates memory for an array of the specified type.

IONewZero

Allocates memory for an array of the specified type and zero-initializes that memory.

IOMalloc

Allocates the specified amount of general-purpose memory.

IOMallocZero

Allocates the specified amount of general-purpose memory and zero-initializes it.

OSTypeAlloc

Allocates memory for a named class.

### Deallocation

IODelete

Frees the memory associated with a valid, typed array.

IOSafeDeleteNULL

Frees the memory associated with a typed array.

OSSafeReleaseNULL

Frees memory that you allocated for a named class.

IOFree

Frees a memory block that contains general-purpose memory.

### Address Utilities

IOVMPageSize

The number of bytes in a virtual memory page.

### Addresses

IOVirtualAddress

An address in the virtual memory space of the process.

IOPhysicalAddress

An address in physical memory.

IOPhysicalAddress32

A 32-bit address in physical memory.

IOPhysicalAddress64

A 64-bit address in physical memory.

IOPhysicalLength

A type that represents the length of a memory block.

IOPhysicalLength32

A type that represents the length of a memory block in a 32-bit address space.

IOPhysicalLength64

A type that represents the length of a memory block in a 64-bit address space.

IOCacheMode

A memory-cache mode.

### Byte Counts

IOByteCount

A type that represents a number of bytes.

IOByteCount32

A type that represents a number of bytes in a 32-bit address space.

IOByteCount64

A type that represents a number of bytes in a 64-bit address space.

## See Also

### Memory management

IOBufferMemoryDescriptor

A memory buffer allocated in the caller’s address space.

IOMemoryDescriptor

The base class for describing a location in memory.

IOMemoryMap

A reference to an existing block of memory in the current process or in a different process.

