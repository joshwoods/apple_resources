

- Paravirtualized Graphics
-  PGReadMemory 

Type Alias

# PGReadMemory

The block signature for a routine that copies data from guest physical memory into host memory.

Mac Catalyst 14.0+macOS 11.0+

``` source
typealias PGReadMemory = (UInt64, UInt64, UnsafeMutableRawPointer) -> Bool
```

## Parameters 

`physicalAddress`  

The physical guest address of the data to read.

`length`  

The number of bytes to read.

`dst`  

The destination for the copied data.

## Return Value

Returns true if the block copied the data successfully; otherwise false.

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

struct PGPhysicalMemoryRange_s

A range in the guest virtual machine’s physical memory address space.

