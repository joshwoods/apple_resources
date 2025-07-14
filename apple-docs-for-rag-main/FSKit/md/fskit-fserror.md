

- FSKit
-  FSError 

Structure

# FSError

An error encountered when performing an FSKit operation.

macOS 15.4+

``` source
struct FSError
```

## Topics

### Identifying errors

static var invalidDirectoryCookie: FSError.Code

static var moduleLoadFailed: FSError.Code

static var resourceDamaged: FSError.Code

static var resourceUnrecognized: FSError.Code

static var resourceUnusable: FSError.Code

static var statusOperationInProgress: FSError.Code

static var statusOperationPaused: FSError.Code

### Identifying the error domain

static var errorDomain: String

The domain of the error.

### Default Implementations

CustomNSError Implementations

Equatable Implementations

Error Implementations

Hashable Implementations

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Errors and logging

func fs_errorForCocoaError(Int32) -> any Error

Creates an error object for the given Cocoa error code.

func fs_errorForMachError(Int32) -> any Error

Creates an error object for the given Mach error code.

func fs_errorForPOSIXError(Int32) -> any Error

Creates an error object for the given POSIX error code.

enum Code

A code that indicates a specific FSKit error.

let FSKitErrorDomain: String

An error domain for FSKit errors.

