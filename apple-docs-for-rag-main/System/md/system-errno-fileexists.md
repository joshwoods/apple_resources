

- System
- Errno
-  fileExists 

Type Property

# fileExists

File exists.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var fileExists: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

An existing file was mentioned in an inappropriate context; for example, as the new link name in a link function.

The corresponding C error is `EEXIST`.

## See Also

### File and Directory Errors

static var attributeNotFound: Errno

Attribute not found.

static var badFileDescriptor: Errno

Bad file descriptor.

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

