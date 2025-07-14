

- DeviceDiscoveryExtension
-  DDErrorOutType 

Type Alias

# DDErrorOutType

A type for framework functions that return error references.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOSvisionOS 1.0+

``` source
typealias DDErrorOutType = AutoreleasingUnsafeMutablePointer
```

## See Also

### Errors

struct DDError

An error that the framework reports.

enum Code

Codes that identify errors that can occur during the framework’s use.

typealias DDErrorHandler

A function that executes code you provide when an operation returns an error or completes successfully.

let DDErrorDomain: String

A unique error domain for the framework.

