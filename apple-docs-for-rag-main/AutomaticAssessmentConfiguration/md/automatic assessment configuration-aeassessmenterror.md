

- Automatic Assessment Configuration
-  AEAssessmentError 

Structure

# AEAssessmentError

Errors issued by an assessment session to its delegate.

iOS 13.4+iPadOS 13.4+Mac Catalyst 14.0+macOS 10.15.4+

``` source
struct AEAssessmentError
```

## Topics

### Error codes

static var unknown: AEAssessmentError.Code

The session encountered an unknown error.

static var unsupportedPlatform: AEAssessmentError.Code

The feature isn’t supported on this platform.

enum Code

Error codes that the framework returns if a session fails.

### Error characteristics

let AEAssessmentErrorDomain: String

A constant representing the error domain that the framework uses when issuing errors.

### Type Properties

static var configurationUpdatesNotSupported: AEAssessmentError.Code

static var errorDomain: String

static var multipleParticipantsNotSupported: AEAssessmentError.Code

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

Error codes that the framework returns if a session fails.

let AEAssessmentErrorDomain: String

A constant representing the error domain that the framework uses when issuing errors.

