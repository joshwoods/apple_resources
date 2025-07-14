

- SafetyKit
-  SAError 

Structure

# SAError

An error reported by SafetyKit.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+watchOS 10.1+

``` source
struct SAError
```

## Topics

### Inspecting error information

var localizedDescription: String

Retrieve the localized description for this error.

static var errorDomain: String

### Comparing errors

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Identifying an error cause

enum Code

Codes for identifying errors in SafetyKit.

let SAErrorDomain: String

The domain for error objects that SafetyKit produces.

static var invalidArgument: SAError.Code

The method received an argument that it can’t validate.

static var notAllowed: SAError.Code

The system currently restricts the feature on this device.

static var notAuthorized: SAError.Code

The system denies the app from performing the requested operation.

static var operationFailed: SAError.Code

The requested operation failed; retrying may succeed.

### Default Implementations

CustomNSError Implementations

Equatable Implementations

Error Implementations

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Handling errors

let SAErrorDomain: String

The domain for error objects that SafetyKit produces.

enum Code

Codes for identifying errors in SafetyKit.

