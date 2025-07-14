

- Apple Archive
- ArchiveByteStream
-  withFileStream(path:mode:options:permissions:\_:) 

Type Method

# withFileStream(path:mode:options:permissions:\_:)

Calls the given closure with a file stream.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func withFileStream(
    path: FilePath,
    mode: FileDescriptor.AccessMode,
    options: FileDescriptor.OpenOptions,
    permissions: FilePermissions,
    _ body: (ArchiveByteStream) throws -> E
) throws -> E
```

## Parameters 

`path`  

The file path.

`mode`  

The file descriptor access mode.

`options`  

The file descriptor options that specify behavior on opening a file.

`permissions`  

The file permission bits that govern access to a file.

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

static func temporaryFileStream() -> ArchiveByteStream?

Creates a new temporary file stream.

static func withTemporaryFileStream&lt;E>((ArchiveByteStream) throws -> E) throws -> E

Calls the given closure with a temporary file stream.

