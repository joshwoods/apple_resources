

- PHASE
-  PHASEError 

Structure

# PHASEError

An error that PHASE reports.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
struct PHASEError
```

## Topics

### Identifying an Error Cause

static var initializeFailed: PHASEError.Code

An error that indicates the engine failed to initialize.

static var invalidObject: PHASEError.Code

An error that indicates an object is invalid in a specific context.

### Creating an Error

enum Code

Codes that identify errors in PHASE.

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

### Framework Errors

enum Code

Codes that identify errors in PHASE.

let PHASEErrorDomain: String

A unique error domain for the framework.

