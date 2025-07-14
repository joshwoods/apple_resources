

- System
- Errno
-  diskQuotaExceeded 

Type Property

# diskQuotaExceeded

Disk quota exceeded.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var diskQuotaExceeded: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

A write to an ordinary file, the creation of a directory or symbolic link, or the creation of a directory entry failed because the user’s quota of disk blocks was exhausted, or the allocation of an inode for a newly created file failed because the user’s quota of inodes was exhausted.

The corresponding C error is `EDQUOT`.

## See Also

### File System Errors

static var badFileTypeOrFormat: Errno

Inappropriate file type or format.

static var directoryNotEmpty: Errno

Directory not empty.

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

