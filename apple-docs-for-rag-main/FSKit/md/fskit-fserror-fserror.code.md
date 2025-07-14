

- FSKit
- FSError
-  FSError.Code 

Enumeration

# FSError.Code

A code that indicates a specific FSKit error.

macOS 15.4+

``` source
enum Code
```

## Topics

### Identifying errors

case invalidDirectoryCookie

While enumerating a directory, the given cookie didn’t resolve to a valid directory entry.

case moduleLoadFailed

The module failed to load.

case resourceDamaged

The resource is damaged.

case resourceUnrecognized

FSKit didn’t recognize the resource, and probing failed to find a match.

case resourceUnusable

FSKit recognizes the resource, but the resource isn’t usable.

case statusOperationInProgress

An operation is in progress.

case statusOperationPaused

An operation is paused.

### Working with raw values

init?(rawValue: Int)

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Errors and logging

func fs_errorForCocoaError(Int32) -> any Error

Creates an error object for the given Cocoa error code.

func fs_errorForMachError(Int32) -> any Error

Creates an error object for the given Mach error code.

func fs_errorForPOSIXError(Int32) -> any Error

Creates an error object for the given POSIX error code.

struct FSError

An error encountered when performing an FSKit operation.

let FSKitErrorDomain: String

An error domain for FSKit errors.

