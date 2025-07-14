

- AVFoundation
-  AVCaptionConversionWarning 

Class

# AVCaptionConversionWarning

An object that represents a conversion warning produced by a validator.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
class AVCaptionConversionWarning
```

## Topics

### Inspecting the Warning

var warningType: AVCaptionConversionWarning.WarningType

A type that indicates the nature of the validation warning.

var rangeOfCaptions: NSRange

The range of the captions for which the system issued a warning.

var adjustment: AVCaptionConversionAdjustment?

A correction the converter makes when it converts a caption to a specific format.

class AVCaptionConversionAdjustment

An object that describes an adjustment to correct a problem found during validation of a caption conversion.

struct WarningType

The type of a caption conversion warning.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Validating Captions

func validateCaptionConversion(warningHandler: (AVCaptionConversionWarning?) -> Void)

Validates the object’s captions.

var warnings: [AVCaptionConversionWarning]

The collection of warnings the validator encountered.

func stopValidating()

Stops the active validation operation.

