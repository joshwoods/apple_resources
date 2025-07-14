

- PHASE
- PHASEError
-  PHASEError.Code 

Enumeration

# PHASEError.Code

Codes that identify errors in PHASE.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
enum Code
```

## Topics

### Errors

case initializeFailed

An error that indicates the engine failed to initialize.

case invalidObject

An error that indicates an object is invalid in a specific context.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Framework Errors

struct PHASEError

An error that PHASE reports.

let PHASEErrorDomain: String

A unique error domain for the framework.

