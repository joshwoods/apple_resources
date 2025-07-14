

- DeviceDiscoveryExtension
-  DDError 

Structure

# DDError

An error that the framework reports.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOSvisionOS 1.0+

``` source
struct DDError
```

## Topics

### Identifying an error cause

enum Code

Codes that identify errors that can occur during the framework’s use.

static var success: DDError.Code

An error that indicates an operation succeeds.

static var unknown: DDError.Code

An error that indicates an uncategorized problem.

static var badParameter: DDError.Code

An error that indicates the framework doesn’t support a parameter that the extension provides.

static var unsupported: DDError.Code

An error that indicates an unsupported configuration.

static var timeout: DDError.Code

An error that indicates a timeout occurs.

static var `internal`: DDError.Code

An error that indicates a problem of internal origin.

static var missingEntitlement: DDError.Code

An error that indicates that the app extension lacks a required entitlement.

static var permission: DDError.Code

An error that indicates the app extension lacks necessary permissions.

static var next: DDError.Code

An error the framework reserves for future use.

### Type Properties

static var errorDomain: String

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Errors

enum Code

Codes that identify errors that can occur during the framework’s use.

typealias DDErrorHandler

A function that executes code you provide when an operation returns an error or completes successfully.

typealias DDErrorOutType

A type for framework functions that return error references.

let DDErrorDomain: String

A unique error domain for the framework.

