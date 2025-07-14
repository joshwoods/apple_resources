

- System
- Errno
-  readOnlyFileSystem 

Type Property

# readOnlyFileSystem

Read-only file system.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var readOnlyFileSystem: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

You attempted to modify a file or directory on a file system that was read-only at the time.

The corresponding C error is `EROFS`.

## See Also

### File System Errors

static var badFileTypeOrFormat: Errno

Inappropriate file type or format.

static var directoryNotEmpty: Errno

Directory not empty.

static var diskQuotaExceeded: Errno

Disk quota exceeded.

static var noSpace: Errno

Device out of space.

static var tooManyLinks: Errno

Too many links.

static var tooManyOpenFilesInSystem: Errno

The system has too many open files.

static var tooManyOpenFiles: Errno

This process has too many open files.

