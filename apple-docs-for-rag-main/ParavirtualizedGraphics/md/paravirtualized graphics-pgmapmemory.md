

- Paravirtualized Graphics
-  PGMapMemory 

Type Alias

# PGMapMemory

The block signature for a routine that maps guest physical memory into a task.

Mac Catalyst 14.0+macOS 11.0+

``` source
typealias PGMapMemory = (OpaquePointer, UInt32, UInt64, Bool, UnsafeMutablePointer) -> Bool
```

## Parameters 

`task`  

The task to map the memory into.

`rangeCount `  

The number of ranges to map.

`virtualOffset `  

The offset from the task’s base address where mapping starts.

`readOnly `  

A Boolean value that indicates whether the block maps memory for read access only.

`ranges `  

The set of ranges to map.

## Return Value

Returns true if the block successfully mapped memory; otherwise false.

## See Also

### Managing Memory Operations

var mapMemory: PGMapMemory?

A handler that the framework calls to map memory into the virtual machine.

var unmapMemory: PGUnmapMemory?

A handler that the framework calls to unmap memory from the virtual machine.

var readMemory: PGReadMemory?

A handler that the framework calls to read data from the guest’s memory.

typealias PGUnmapMemory

The block signature for a routine that unmaps guest physical memory from a task.

typealias PGReadMemory

The block signature for a routine that copies data from guest physical memory into host memory.

struct PGPhysicalMemoryRange_s

A range in the guest virtual machine’s physical memory address space.

