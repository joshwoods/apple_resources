

- ARKit
- ARKitSession
- ARKitSession.Error
-  ARKitSession.Error.Code 

Enumeration

# ARKitSession.Error.Code

The error codes for ARKit sessions.

visionOS 1.0+

``` source
enum Code
```

## Topics

### Determining the cause of session errors

case dataProviderFailedToRun

The error code for when a data provider fails to run.

case dataProviderNotAuthorized

The error code for when a data provider is missing at least one authorization it needs to run.

### Instance Properties

var description: String

A textual representation of the code.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Hashable

## See Also

### Inspecting ARKit errors

let dataProvider: (any DataProvider)?

The data provider that caused an error in a session.

var code: ARKitSession.Error.Code

The error code for an ARKit session error.

var errorDescription: String?

A localized message that describes the error that occurred.

