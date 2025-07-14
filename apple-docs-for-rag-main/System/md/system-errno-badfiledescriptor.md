

- System
- Errno
-  badFileDescriptor 

Type Property

# badFileDescriptor

Bad file descriptor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var badFileDescriptor: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

A file descriptor argument was out of range, referred to no open file, or a read (write) request was made to a file that was only open for writing (reading).

The corresponding C error is `EBADF`.

## See Also

### File and Directory Errors

static var attributeNotFound: Errno

Attribute not found.

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

static var permissionDenied: Errno

Permission denied.

static var textFileBusy: Errno

Text file busy.

