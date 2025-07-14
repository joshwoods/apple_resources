

- Paravirtualized Graphics
- PGDeviceDescriptor
-  readMemory 

Instance Property

# readMemory

A handler that the framework calls to read data from the guest’s memory.

Mac Catalyst 14.0+macOS 11.0+

``` source
var readMemory: PGReadMemory? { get set }
```

## See Also

### Managing Memory Operations

var mapMemory: PGMapMemory?

A handler that the framework calls to map memory into the virtual machine.

var unmapMemory: PGUnmapMemory?

A handler that the framework calls to unmap memory from the virtual machine.

typealias PGMapMemory

The block signature for a routine that maps guest physical memory into a task.

typealias PGUnmapMemory

The block signature for a routine that unmaps guest physical memory from a task.

typealias PGReadMemory

The block signature for a routine that copies data from guest physical memory into host memory.

struct PGPhysicalMemoryRange_s

A range in the guest virtual machine’s physical memory address space.

