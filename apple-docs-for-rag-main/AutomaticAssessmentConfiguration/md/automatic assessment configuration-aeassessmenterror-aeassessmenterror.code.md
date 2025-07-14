

- Automatic Assessment Configuration
- AEAssessmentError
-  AEAssessmentError.Code 

Enumeration

# AEAssessmentError.Code

Error codes that the framework returns if a session fails.

iOS 13.4+iPadOS 13.4+Mac Catalyst 14.0+macOS 10.15.4+

``` source
enum Code
```

## Topics

### Possible errors

case configurationUpdatesNotSupported

An active session fails to update its configuration because configuration updates are not supported by the current device or platform.

case multipleParticipantsNotSupported

A session fails to begin or update with a configuration that contains one or more participant applications because mulitple participant configurations are not supported by the device or platform.

case unknown

The session encountered an unknown error.

case unsupportedPlatform

The feature isn’t supported on this platform.

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

### Errors

struct AEAssessmentError

Errors issued by an assessment session to its delegate.

let AEAssessmentErrorDomain: String

A constant representing the error domain that the framework uses when issuing errors.

