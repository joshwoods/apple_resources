

- Dispatch
- DispatchIO
-  DispatchIO.StreamType 

Enumeration

# DispatchIO.StreamType

The semantics for accessing the contents of a file descriptor.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum StreamType
```

## Topics

### Stream Types

case stream

Access content sequentially, in a stream.

case random

Access content randomly.

### Initializing the Type

var DISPATCH_IO_RANDOM: Int32

var DISPATCH_IO_STREAM: Int32

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating a Dispatch I/O Object

convenience init(type: DispatchIO.StreamType, fileDescriptor: Int32, queue: DispatchQueue, cleanupHandler: (Int32) -> Void)

Creates a new I/O channel that accesses the specified file descriptor.

convenience init?(type: DispatchIO.StreamType, path: UnsafePointer&lt;Int8>, oflag: Int32, mode: mode_t, queue: DispatchQueue, cleanupHandler: (Int32) -> Void)

Creates a new I/O channel that accesses the file at the specified path, potentially creating that file in the process.

convenience init(type: DispatchIO.StreamType, io: DispatchIO, queue: DispatchQueue, cleanupHandler: (Int32) -> Void)

Creates a new I/O channel from an existing I/O channel.

