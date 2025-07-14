

- Background Assets
-  BAErrorCode 

Enumeration

# BAErrorCode

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 18.4+visionOS 2.4+

``` source
enum BAErrorCode
```

## Topics

### Error codes

case callFromExtensionNotAllowed

case callFromInactiveProcessNotAllowed

case callerConnectionInvalid

case callerConnectionNotAccepted

case downloadAlreadyFailed

case downloadAlreadyScheduled

case downloadBackgroundActivityProhibited

case downloadEssentialDownloadNotPermitted

case downloadFailedToStart

case downloadInvalid

case downloadNotScheduled

case downloadWouldExceedAllowance

case sessionDownloadAllowanceExceeded

case sessionDownloadDisallowedByAllowance

case sessionDownloadDisallowedByDomain

case sessionDownloadNotPermittedBeforeAppLaunch

### Enumeration Cases

case downloadDoesNotExist

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

let BAErrorDomain: String

