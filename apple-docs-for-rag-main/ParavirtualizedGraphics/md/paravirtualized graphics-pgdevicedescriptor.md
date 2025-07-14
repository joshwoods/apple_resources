

- Paravirtualized Graphics
-  PGDeviceDescriptor 

Class

# PGDeviceDescriptor

A description of the paravirtualized graphics device to create.

Mac Catalyst 14.0+macOS 11.0+

``` source
class PGDeviceDescriptor
```

## Topics

### Specifying the GPU

var device: (any MTLDevice)?

The Metal device object to use to back the virtual graphics device.

### Managing Tasks

var createTask: PGCreateTask?

A handler that the framework calls to create a task object.

var destroyTask: PGDestroyTask?

A handler that the framework calls to destroy a task object.

typealias PGCreateTask

The block signature for a routine that creates a task.

typealias PGDestroyTask

The block signature for a routine that destroys a task.

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

struct PGPhysicalMemoryRange_s

A range in the guest virtual machine’s physical memory address space.

### Specifying Trace Behavior

var addTraceRange: PGAddTraceRange?

A handler that the framework calls to add a trace range.

var removeTraceRange: PGRemoveTraceRange?

A handler that the framework calls to remove a trace range.

typealias PGAddTraceRange

The block signature for a routine that adds a trace range.

typealias PGRemoveTraceRange

The block signature for a routine that removes a trace range.

typealias PGTraceRangeHandler

The block signature for a routine that handles trace requests.

### Handling Interrupts

var raiseInterrupt: PGRaiseInterrupt?

A handler that the system calls to raise an interrupt in the guest environment.

typealias PGRaiseInterrupt

The block signature for a routine that raises interrupts in the guest environment.

### Specifying Virtual Device Properties

var mmioLength: Int

The length in bytes of the memory-mapped IO section.

### Instance Properties

var displayPortCount: UInt32

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Devices

func PGNewDeviceWithDescriptor(PGDeviceDescriptor) -> (any PGDevice)?

Creates a new paravirtualized graphics device.

protocol PGDevice

A paravirtualized GPU device object.

