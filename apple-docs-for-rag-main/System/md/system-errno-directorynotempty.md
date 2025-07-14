

- System
- Errno
-  directoryNotEmpty 

Type Property

# directoryNotEmpty

Directory not empty.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var directoryNotEmpty: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

A directory with entries other than `.` and `..` was supplied to a `remove(2)` directory or `rename(2)` call.

The corresponding C error is `ENOTEMPTY`.

## See Also

### File System Errors

static var badFileTypeOrFormat: Errno

Inappropriate file type or format.

static var diskQuotaExceeded: Errno

Disk quota exceeded.

static var noSpace: Errno

Device out of space.

static var readOnlyFileSystem: Errno

Read-only file system.

static var tooManyLinks: Errno

Too many links.

static var tooManyOpenFilesInSystem: Errno

The system has too many open files.

static var tooManyOpenFiles: Errno

This process has too many open files.

