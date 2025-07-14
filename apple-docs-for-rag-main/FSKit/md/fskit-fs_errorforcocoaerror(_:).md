

- FSKit
-  fs_errorForCocoaError(\_:) 

Function

# fs_errorForCocoaError(\_:)

Creates an error object for the given Cocoa error code.

macOS 15.4+

``` source
func fs_errorForCocoaError(_ errorCode: Int32) -> any Error
```

## See Also

### Errors and logging

func fs_errorForMachError(Int32) -> any Error

Creates an error object for the given Mach error code.

func fs_errorForPOSIXError(Int32) -> any Error

Creates an error object for the given POSIX error code.

struct FSError

An error encountered when performing an FSKit operation.

enum Code

A code that indicates a specific FSKit error.

let FSKitErrorDomain: String

An error domain for FSKit errors.

