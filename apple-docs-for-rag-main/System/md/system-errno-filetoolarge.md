

- System
- Errno
-  fileTooLarge 

Type Property

# fileTooLarge

The file is too large.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var fileTooLarge: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

The file exceeds the maximum size allowed by the file system. For example, the maximum size on UFS is about 2.1 gigabytes, and about 9,223 petabytes on HFS-Plus and Apple File System.

The corresponding C error is `EFBIG`.

## See Also

### File and Directory Errors

static var attributeNotFound: Errno

Attribute not found.

static var badFileDescriptor: Errno

Bad file descriptor.

static var fileExists: Errno

File exists.

static var improperLink: Errno

Improper link.

static var isDirectory: Errno

Is a directory.

static var noLocks: Errno

No locks available.

static var noSuchFileOrDirectory: Errno

No such file or directory.

static var notDirectory: Errno

Not a directory.

static var permissionDenied: Errno

Permission denied.

static var textFileBusy: Errno

Text file busy.

