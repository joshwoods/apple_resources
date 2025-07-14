

- ARKit
- ObjectTrackingProvider
- ObjectTrackingProvider.Error
-  ObjectTrackingProvider.Error.Code 

Enumeration

# ObjectTrackingProvider.Error.Code

The enumeration of object-tracking provider error codes.

visionOS 2.0+

``` source
enum Code
```

## Topics

### Error codes

case referenceObjectLoadingFailed

Values that indicate loading a reference object model failed.

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

### Describing an error

var code: ObjectTrackingProvider.Error.Code

The error code.

var errorDescription: String?

A localized message that describes an error.

var failureReason: String?

A localized message that describes the reason for the failure.

