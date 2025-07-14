

- FSKit
-  FSKitErrorDomain 

Global Variable

# FSKitErrorDomain

An error domain for FSKit errors.

macOS 15.4+

``` source
let FSKitErrorDomain: String
```

## Discussion

See NSError for more information on error domains.

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

enum Code

A code that indicates a specific FSKit error.

