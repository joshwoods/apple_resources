

- System
- Errno
-  tooManyLinks 

Type Property

# tooManyLinks

Too many links.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var tooManyLinks: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

The maximum number of hard links to a single file (32767) has been exceeded.

The corresponding C error is `EMLINK`.

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

static var readOnlyFileSystem: Errno

Read-only file system.

static var tooManyOpenFilesInSystem: Errno

The system has too many open files.

static var tooManyOpenFiles: Errno

This process has too many open files.

