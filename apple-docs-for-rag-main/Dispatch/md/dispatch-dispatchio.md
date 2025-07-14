

- Dispatch
-  DispatchIO 

Class

# DispatchIO

An object that manages operations on a file descriptor using either stream-based or random-access semantics.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class DispatchIO
```

## Topics

### Creating a Dispatch I/O Object

convenience init(type: DispatchIO.StreamType, fileDescriptor: Int32, queue: DispatchQueue, cleanupHandler: (Int32) -> Void)

Creates a new I/O channel that accesses the specified file descriptor.

convenience init?(type: DispatchIO.StreamType, path: UnsafePointer&lt;Int8>, oflag: Int32, mode: mode_t, queue: DispatchQueue, cleanupHandler: (Int32) -> Void)

Creates a new I/O channel that accesses the file at the specified path, potentially creating that file in the process.

convenience init(type: DispatchIO.StreamType, io: DispatchIO, queue: DispatchQueue, cleanupHandler: (Int32) -> Void)

Creates a new I/O channel from an existing I/O channel.

enum StreamType

The semantics for accessing the contents of a file descriptor.

### Reading from the File

func read(offset: off_t, length: Int, queue: DispatchQueue, ioHandler: (Bool, DispatchData?, Int32) -> Void)

Schedules an asynchronous read operation on the specified channel.

class func read(fromFileDescriptor: Int32, maxLength: Int, runningHandlerOn: DispatchQueue, handler: (DispatchData, Int32) -> Void)

Schedules an asynchronous read operation using the specified file descriptor.

### Writing to the File

func write(offset: off_t, data: DispatchData, queue: DispatchQueue, ioHandler: (Bool, DispatchData?, Int32) -> Void)

Schedules an asynchronous write operation for the specified channel.

class func write(toFileDescriptor: Int32, data: DispatchData, runningHandlerOn: DispatchQueue, handler: (DispatchData?, Int32) -> Void)

Schedules an asynchronous write operation to the specified file descriptor.

### Closing the File

func close(flags: DispatchIO.CloseFlags)

Closes the channel to new read and write operations.

struct CloseFlags

Additional flags to use when closing an I/O channel.

### Managing the File Descriptor

var fileDescriptor: Int32

Returns the file descriptor associated with the specified channel.

func setLimit(highWater: Int)

Sets the maximum number of bytes to process before enqueueing a handler block.

func setLimit(lowWater: Int)

Sets the minimum number of bytes to process before enqueueing a handler block.

func setInterval(interval: DispatchTimeInterval, flags: DispatchIO.IntervalFlags)

Sets the interval, in nanoseconds, at which to invoke the I/O handlers for the channel.

struct IntervalFlags

The desired delivery behavior for interval events.

### Synchronizing File Operations

func barrier(execute: () -> Void)

Schedules a barrier operation on the specified channel.

### Initializers

convenience init(type: DispatchIO.StreamType, path: UnsafePointer&lt;Int8>, oflag: Int32, mode: mode_t, queue: DispatchQueue, cleanupHandler: (Int32) -> Void)

## Relationships

### Inherits From

- DispatchObject

### Conforms To

- CVarArg
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### System Event Monitoring

class DispatchSource

An object that coordinates the processing of specific low-level system events, such as file-system events, timers, and UNIX signals.

Dispatch Source

An object that coordinates the processing of specific low-level system events, such as file-system events, timers, and UNIX signals.

struct DispatchData

An object that manages a memory-based data buffer and exposes it as a contiguous block of memory.

struct DispatchDataIterator

A byte-by-byte iterator over the contents of a dispatch data object.

Dispatch I/O

An object that manages operations on a file descriptor using either stream-based or random-access semantics.

Dispatch Data

An object that manages a memory-based data buffer and exposes it as a contiguous block of memory.

protocol DispatchSourceProtocol

Defines a common set of properties and methods that are shared with all dispatch source types.

