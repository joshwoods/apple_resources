

- System
- Errno
-  tooManyOpenFiles 

Type Property

# tooManyOpenFiles

This process has too many open files.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var tooManyOpenFiles: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

To check the current limit, call the `getdtablesize` function.

The corresponding C error is `EMFILE`.

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

static var tooManyLinks: Errno

Too many links.

static var tooManyOpenFilesInSystem: Errno

The system has too many open files.

