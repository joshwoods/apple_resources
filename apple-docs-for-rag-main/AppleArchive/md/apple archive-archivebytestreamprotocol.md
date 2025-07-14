

- Apple Archive
-  ArchiveByteStreamProtocol 

Protocol

# ArchiveByteStreamProtocol

A set of methods that defines the interface for using an archive stream that reads from and writes to buffers.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
protocol ArchiveByteStreamProtocol
```

## Topics

### Reading and Writing Data

func read(into: UnsafeMutableRawBufferPointer) throws -> Int

Reads data to the specified buffer, not exceeding the buffer’s previously allocated size.

**Required**

func read(into: UnsafeMutableRawBufferPointer, atOffset: Int64) throws -> Int

Reads data at the supplied offset to the specified buffer, not exceeding the buffer’s previously allocated size.

**Required**

func write(from: UnsafeRawBufferPointer) throws -> Int

Writes data from the specified buffer, not exceeding the buffer’s allocated size.

**Required**

func write(from: UnsafeRawBufferPointer, atOffset: Int64) throws -> Int

Writes data at the supplied offset from the specified buffer, not exceeding the buffer’s allocated size.

**Required**

### Using Archive Byte Streams

func seek(toOffset: Int64, relativeTo: FileDescriptor.SeekOrigin) throws -> Int64

Updates the internal stream position to the specified offset relative to the specified origin.

**Required**

func cancel()

Cancels stream operations.

**Required**

func close() throws

Closes the stream and releases associated resources.

**Required**

## Relationships

### Conforming Types

- ArchiveByteStream

## See Also

### Apple Archive streams

protocol ArchiveStreamProtocol

A set of methods that defines the interface for using an archive stream that reads from and writes to data blobs.

class ArchiveStream

An archive stream that reads from and writes to data blobs

class ArchiveByteStream

An archive stream that reads from and writes to buffers.

