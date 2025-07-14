

- Metal
-  MTLCaptureError 

Enumeration

# MTLCaptureError

Errors returned by capture sessions.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
enum MTLCaptureError
```

## Topics

### Errors

case alreadyCapturing

A capture session is already in progress.

case invalidDescriptor

The descriptor contained invalid parameters.

case notSupported

The requested capture options are not available.

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

### Capture Errors

let MTLCaptureErrorDomain: String

The error domain for capture errors.

