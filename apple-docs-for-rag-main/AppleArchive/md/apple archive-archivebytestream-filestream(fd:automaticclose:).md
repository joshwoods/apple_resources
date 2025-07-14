

- Apple Archive
- ArchiveByteStream
-  fileStream(fd:automaticClose:) 

Type Method

# fileStream(fd:automaticClose:)

Creates a stream from an open file descriptor.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func fileStream(
    fd: FileDescriptor,
    automaticClose: Bool = true
) -> ArchiveByteStream?
```

## Parameters 

`fd`  

The file descriptor that you have previously opened with `open(2)`.

`automaticClose`  

A Boolean value that specifies whether to close the file descriptor when you close the stream.

## Return Value

A new archive byte stream.

## See Also

### File Streaming

static func withFileStream&lt;E>(fd: FileDescriptor, automaticClose: Bool, (ArchiveByteStream) throws -> E) throws -> E

Calls the given closure with a file stream created from the specified file descriptor.

static func fileStream(path: FilePath, mode: FileDescriptor.AccessMode, options: FileDescriptor.OpenOptions, permissions: FilePermissions) -> ArchiveByteStream?

Opens a new file descriptor using the given path and parameters, and creates a stream from the file descriptor.

static func withFileStream&lt;E>(path: FilePath, mode: FileDescriptor.AccessMode, options: FileDescriptor.OpenOptions, permissions: FilePermissions, (ArchiveByteStream) throws -> E) throws -> E

Calls the given closure with a file stream.

static func temporaryFileStream() -> ArchiveByteStream?

Creates a new temporary file stream.

static func withTemporaryFileStream&lt;E>((ArchiveByteStream) throws -> E) throws -> E

Calls the given closure with a temporary file stream.

