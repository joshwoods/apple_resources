

- Apple Archive
- ArchiveByteStream
-  withTemporaryFileStream(\_:) 

Type Method

# withTemporaryFileStream(\_:)

Calls the given closure with a temporary file stream.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func withTemporaryFileStream(_ body: (ArchiveByteStream) throws -> E) throws -> E
```

## Parameters 

`body`  

A closure with the archive byte stream passed as a parameter.

## Return Value

The result of the closure.

## See Also

### File Streaming

static func fileStream(fd: FileDescriptor, automaticClose: Bool) -> ArchiveByteStream?

Creates a stream from an open file descriptor.

static func withFileStream&lt;E>(fd: FileDescriptor, automaticClose: Bool, (ArchiveByteStream) throws -> E) throws -> E

Calls the given closure with a file stream created from the specified file descriptor.

static func fileStream(path: FilePath, mode: FileDescriptor.AccessMode, options: FileDescriptor.OpenOptions, permissions: FilePermissions) -> ArchiveByteStream?

Opens a new file descriptor using the given path and parameters, and creates a stream from the file descriptor.

static func withFileStream&lt;E>(path: FilePath, mode: FileDescriptor.AccessMode, options: FileDescriptor.OpenOptions, permissions: FilePermissions, (ArchiveByteStream) throws -> E) throws -> E

Calls the given closure with a file stream.

static func temporaryFileStream() -> ArchiveByteStream?

Creates a new temporary file stream.

