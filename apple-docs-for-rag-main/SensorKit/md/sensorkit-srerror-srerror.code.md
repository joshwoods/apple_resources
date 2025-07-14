

- SensorKit
- SRError
-  SRError.Code 

Enumeration

# SRError.Code

The kinds of problems that stop a recording or a fetch.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
enum Code
```

## Topics

### Errors

case promptDeclined

Occurs when the user cancels the sensor approval workflow.

case dataInaccessible

Occurs when the app can’t access the sensor’s data.

case fetchRequestInvalid

Occurs when the app misconfigures a fetch request.

case invalidEntitlement

Occurs when the app lacks the required entitlement.

case noAuthorization

Occurs when the user declines sensor access in the Settings app.

### Creating an error

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Interpreting Errors

let SRErrorDomain: String

An error domain that’s unique to the framework.

struct SRError

An error that SensorKit reports.

