

- AVFoundation
- AVCaptionConversionWarning
-  AVCaptionConversionWarning.WarningType 

Structure

# AVCaptionConversionWarning.WarningType

The type of a caption conversion warning.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
struct WarningType
```

## Topics

### Warning Types

static let excessMediaData: AVCaptionConversionWarning.WarningType

A type that indicates one or more captions exceed the media data capacity for media of the type and subtype that the conversion settings specify.

### Initializers

init(rawValue: String)

Creates a warning type with a string.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting the Warning

var warningType: AVCaptionConversionWarning.WarningType

A type that indicates the nature of the validation warning.

var rangeOfCaptions: NSRange

The range of the captions for which the system issued a warning.

var adjustment: AVCaptionConversionAdjustment?

A correction the converter makes when it converts a caption to a specific format.

class AVCaptionConversionAdjustment

An object that describes an adjustment to correct a problem found during validation of a caption conversion.

