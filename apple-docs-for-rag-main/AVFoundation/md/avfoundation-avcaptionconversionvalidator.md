

- AVFoundation
-  AVCaptionConversionValidator 

Class

# AVCaptionConversionValidator

An object that validates captions for a conversion operation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
class AVCaptionConversionValidator
```

## Topics

### Creating a Validator

init(captions: [AVCaption], timeRange: CMTimeRange, conversionSettings: [AVCaptionSettingsKey : Any])

Creates an object that validates captions for a conversion operation.

### Inspecting the Validator

var captions: [AVCaption]

The array of captions that the system validates.

var timeRange: CMTimeRange

The time range of the media timeline in which the captions must exist.

### Validating Captions

func validateCaptionConversion(warningHandler: (AVCaptionConversionWarning?) -> Void)

Validates the object’s captions.

var warnings: [AVCaptionConversionWarning]

The collection of warnings the validator encountered.

class AVCaptionConversionWarning

An object that represents a conversion warning produced by a validator.

func stopValidating()

Stops the active validation operation.

### Checking the Status

var status: AVCaptionConversionValidator.Status

A value that indicates the status of validation.

enum Status

Constants that indicate the status of a validator.

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

## See Also

### Conversion and Validation

struct AVCaptionSettingsKey

A structure that defines dictionary keys to configure the caption converter and validator.

class AVCaptionFormatConformer

An object that converts a canonical caption to a specific format.

