

- System
- Errno
-  textFileBusy 

Type Property

# textFileBusy

Text file busy.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var textFileBusy: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

The new process was a pure procedure (shared text) file, which was already open for writing by another process, or while the pure procedure file was being executed, an open call requested write access.

The corresponding C error is `ETXTBSY`.

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

static var permissionDenied: Errno

Permission denied.

