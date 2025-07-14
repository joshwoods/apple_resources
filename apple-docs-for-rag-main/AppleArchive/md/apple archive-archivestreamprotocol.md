

- Apple Archive
-  ArchiveStreamProtocol 

Protocol

# ArchiveStreamProtocol

A set of methods that defines the interface for using an archive stream that reads from and writes to data blobs.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
protocol ArchiveStreamProtocol
```

## Topics

### Reading and Writing Blobs

func readBlob(key: ArchiveHeader.FieldKey, into: UnsafeMutableRawBufferPointer) throws

Reads the current entry blob data.

**Required**

func writeBlob(key: ArchiveHeader.FieldKey, from: UnsafeRawBufferPointer) throws

Writes an entry blob data.

**Required**

### Reading and Writing Headers

func readHeader() throws -> ArchiveHeader?

Reads the next entry header.

**Required**

func writeHeader(ArchiveHeader) throws

Writes an entry header.

**Required**

### Using Archive Streams

func cancel()

Cancels stream operations.

**Required**

func close() throws

Closes the stream and releases associated resources.

**Required**

## Relationships

### Conforming Types

- ArchiveStream

## See Also

### Apple Archive streams

class ArchiveStream

An archive stream that reads from and writes to data blobs

protocol ArchiveByteStreamProtocol

A set of methods that defines the interface for using an archive stream that reads from and writes to buffers.

class ArchiveByteStream

An archive stream that reads from and writes to buffers.

