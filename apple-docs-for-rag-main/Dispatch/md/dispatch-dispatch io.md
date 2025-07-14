

- Dispatch
-  Dispatch I/O 

API Collection

# Dispatch I/O

An object that manages operations on a file descriptor using either stream-based or random-access semantics.

## Topics

### Creating a Dispatch I/O Object

typealias dispatch_io_t

A dispatch I/O channel.

### Managing the File Descriptor

var fileDescriptor: Int32

Returns the file descriptor associated with the specified channel.

func setLimit(lowWater: Int)

Sets the minimum number of bytes to process before enqueueing a handler block.

func setLimit(highWater: Int)

Sets the maximum number of bytes to process before enqueueing a handler block.

### Synchronizing File Operations

func barrier(execute: () -> Void)

Schedules a barrier operation on the specified channel.

## See Also

### System Event Monitoring

class DispatchSource

An object that coordinates the processing of specific low-level system events, such as file-system events, timers, and UNIX signals.

Dispatch Source

An object that coordinates the processing of specific low-level system events, such as file-system events, timers, and UNIX signals.

class DispatchIO

An object that manages operations on a file descriptor using either stream-based or random-access semantics.

struct DispatchData

An object that manages a memory-based data buffer and exposes it as a contiguous block of memory.

struct DispatchDataIterator

A byte-by-byte iterator over the contents of a dispatch data object.

Dispatch Data

An object that manages a memory-based data buffer and exposes it as a contiguous block of memory.

protocol DispatchSourceProtocol

Defines a common set of properties and methods that are shared with all dispatch source types.

