

- Paravirtualized Graphics
-  PGPhysicalMemoryRange_s 

Structure

# PGPhysicalMemoryRange_s

A range in the guest virtual machine’s physical memory address space.

Mac Catalyst 14.0+macOS 11.0+

``` source
struct PGPhysicalMemoryRange_s
```

## Topics

### Creating a Memory Range

init()

Creates a default memory range.

init(physicalAddress: UInt64, physicalLength: UInt64)

Creates a memory range.

### Inspecting Range Properties

var physicalAddress: UInt64

The starting address of the range in physical memory.

var physicalLength: UInt64

The length of the range.

### Type alias

typealias PGPhysicalMemoryRange_t

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Managing Memory Operations

var mapMemory: PGMapMemory?

A handler that the framework calls to map memory into the virtual machine.

var unmapMemory: PGUnmapMemory?

A handler that the framework calls to unmap memory from the virtual machine.

var readMemory: PGReadMemory?

A handler that the framework calls to read data from the guest’s memory.

typealias PGMapMemory

The block signature for a routine that maps guest physical memory into a task.

typealias PGUnmapMemory

The block signature for a routine that unmaps guest physical memory from a task.

typealias PGReadMemory

The block signature for a routine that copies data from guest physical memory into host memory.

