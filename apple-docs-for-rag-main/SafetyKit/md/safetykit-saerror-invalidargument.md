

- SafetyKit
- SAError
-  invalidArgument 

Type Property

# invalidArgument

The method received an argument that it can’t validate.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+watchOS 10.1+

``` source
static var invalidArgument: SAError.Code { get }
```

## See Also

### Identifying an error cause

enum Code

Codes for identifying errors in SafetyKit.

let SAErrorDomain: String

The domain for error objects that SafetyKit produces.

static var notAllowed: SAError.Code

The system currently restricts the feature on this device.

static var notAuthorized: SAError.Code

The system denies the app from performing the requested operation.

static var operationFailed: SAError.Code

The requested operation failed; retrying may succeed.

