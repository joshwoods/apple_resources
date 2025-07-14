

- ARKit
- ARKitSession
-  ARKitSession.Error 

Structure

# ARKitSession.Error

An error that might occur when running data providers on an ARKit session.

visionOS 1.0+

``` source
struct Error
```

## Topics

### Inspecting ARKit errors

let dataProvider: (any DataProvider)?

The data provider that caused an error in a session.

var code: ARKitSession.Error.Code

The error code for an ARKit session error.

enum Code

The error codes for ARKit sessions.

var errorDescription: String?

A localized message that describes the error that occurred.

### Providing recovery suggestions

var recoverySuggestion: String?

A localized message that describes how someone might recover from the error.

var failureReason: String?

A localized message that describes why the error occurred.

### Instance Properties

var description: String

A textual representation of this error.

## Relationships

### Conforms To

- CustomStringConvertible
- Error
- LocalizedError
- Sendable

## See Also

### Starting and stopping a session

convenience init()

Creates a new session.

func run([any DataProvider]) async throws

Runs a session with the data providers you supply.

func stop()

Stops all data providers running in this session.

