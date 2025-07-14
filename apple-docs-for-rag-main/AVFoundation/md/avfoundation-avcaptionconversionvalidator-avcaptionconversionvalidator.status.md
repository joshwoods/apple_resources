

- AVFoundation
- AVCaptionConversionValidator
-  AVCaptionConversionValidator.Status 

Enumeration

# AVCaptionConversionValidator.Status

Constants that indicate the status of a validator.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
enum Status
```

## Topics

### Validation Statuses

case unknown

A status that indicates the system didn’t initialize the validation operation.

case validating

A status that indicates the system validation is in progress.

case completed

A status that indicates the system validation is complete.

case stopped

A status that indicates the system validation stopped prior to completion.

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

### Checking the Status

var status: AVCaptionConversionValidator.Status

A value that indicates the status of validation.

