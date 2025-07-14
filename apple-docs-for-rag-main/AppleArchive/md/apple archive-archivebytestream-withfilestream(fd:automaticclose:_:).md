

- Apple Archive
- ArchiveByteStream
-  withFileStream(fd:automaticClose:\_:) 

Type Method

# withFileStream(fd:automaticClose:\_:)

Calls the given closure with a file stream created from the specified file descriptor.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func withFileStream(
    fd: FileDescriptor,
    automaticClose: Bool = true,
    _ body: (ArchiveByteStream) throws -> E
) throws -> E
```

## Parameters 

`fd`  

The file descriptor that you have previously opened with `open(2)`.

`automaticClose`  

A Boolean value that specifies whether to close the file descriptor when you close the stream.

`body`  

A closure with the archive byte stream passed as a parameter.

## Return Value

The result of the closure.

## See Also

### File Streaming

static func fileStream(fd: FileDescriptor, automaticClose: Bool) -> ArchiveByteStream?

Creates a stream from an open file descriptor.

static func fileStream(path: FilePath, mode: FileDescriptor.AccessMode, options: FileDescriptor.OpenOptions, permissions: FilePermissions) -> ArchiveByteStream?

Opens a new file descriptor using the given path and parameters, and creates a stream from the file descriptor.

static func withFileStream&lt;E>(path: FilePath, mode: FileDescriptor.AccessMode, options: FileDescriptor.OpenOptions, permissions: FilePermissions, (ArchiveByteStream) throws -> E) throws -> E

Calls the given closure with a file stream.

static func temporaryFileStream() -> ArchiveByteStream?

Creates a new temporary file stream.

static func withTemporaryFileStream&lt;E>((ArchiveByteStream) throws -> E) throws -> E

Calls the given closure with a temporary file stream.

