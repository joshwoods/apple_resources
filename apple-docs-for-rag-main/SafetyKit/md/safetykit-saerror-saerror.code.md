

- SafetyKit
- SAError
-  SAError.Code 

Enumeration

# SAError.Code

Codes for identifying errors in SafetyKit.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+watchOS 10.1+

``` source
enum Code
```

## Topics

### Determining the error type

case invalidArgument

The passed argument is invalid.

case notAllowed

The system restricts the feature on this iPhone at the current time.

case notAuthorized

The app isn’t authorized to perform the requested operation.

case operationFailed

The requested operation failed; retrying may succeed.

### Initializers

init?(rawValue: Int)

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Handling errors

let SAErrorDomain: String

The domain for error objects that SafetyKit produces.

struct SAError

An error reported by SafetyKit.

