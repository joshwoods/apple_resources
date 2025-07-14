

- System
- Errno
-  noLocks 

Type Property

# noLocks

No locks available.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var noLocks: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

You have reached the system-imposed limit on the number of simultaneous files.

The corresponding C error is `ENOLCK`.

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

static var noSuchFileOrDirectory: Errno

No such file or directory.

static var notDirectory: Errno

Not a directory.

static var permissionDenied: Errno

Permission denied.

static var textFileBusy: Errno

Text file busy.

