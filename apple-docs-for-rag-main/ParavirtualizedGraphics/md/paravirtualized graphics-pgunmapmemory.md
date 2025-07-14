

- Paravirtualized Graphics
-  PGUnmapMemory 

Type Alias

# PGUnmapMemory

The block signature for a routine that unmaps guest physical memory from a task.

Mac Catalyst 14.0+macOS 11.0+

``` source
typealias PGUnmapMemory = (OpaquePointer, UInt64, UInt64) -> Bool
```

## Parameters 

`task`  

The task to unmap memory from.

`virtualOffset`  

The offset from the task’s base address where unmapping starts.

`length`  

The number of bytes to unmap.

## Return Value

Returns true if the block successfully unmapped memory; otherwise false.

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

typealias PGReadMemory

The block signature for a routine that copies data from guest physical memory into host memory.

struct PGPhysicalMemoryRange_s

A range in the guest virtual machine’s physical memory address space.

