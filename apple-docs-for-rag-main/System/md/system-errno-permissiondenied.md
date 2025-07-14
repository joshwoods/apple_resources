

- System
- Errno
-  permissionDenied 

Type Property

# permissionDenied

Permission denied.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var permissionDenied: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

You attempted to access a file in a way that’s forbidden by the file’s access permissions.

The corresponding C error is `EACCES`.

## See Also

### File and Directory Errors

static var attributeNotFound: Errno

Attribute not found.

static var badFileDescriptor: Errno

Bad file descriptor.

static var fileExists: Errno

File exists.

static var fileTooLarge: Errno

The file is too large.

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

static var textFileBusy: Errno

Text file busy.

