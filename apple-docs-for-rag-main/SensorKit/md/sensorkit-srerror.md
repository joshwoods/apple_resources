

- SensorKit
-  SRError 

Structure

# SRError

An error that SensorKit reports.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
struct SRError
```

## Topics

### Inspecting Error Information

static var errorDomain: String

### Identifying an Error Cause

static var promptDeclined: SRError.Code

Occurs when the user cancels the sensor approval workflow.

static var dataInaccessible: SRError.Code

Occurs when the app can’t access the sensor’s data.

static var fetchRequestInvalid: SRError.Code

Occurs when the app misconfigures a fetch request.

static var invalidEntitlement: SRError.Code

Occurs when the app lacks the required entitlement.

static var noAuthorization: SRError.Code

Occurs when the user declines sensor access in the Settings app.

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Interpreting Errors

let SRErrorDomain: String

An error domain that’s unique to the framework.

enum Code

The kinds of problems that stop a recording or a fetch.

