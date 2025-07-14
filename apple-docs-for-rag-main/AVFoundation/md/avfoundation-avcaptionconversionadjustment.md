

- AVFoundation
-  AVCaptionConversionAdjustment 

Class

# AVCaptionConversionAdjustment

An object that describes an adjustment to correct a problem found during validation of a caption conversion.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
class AVCaptionConversionAdjustment
```

## Topics

### Accessing the Adjustment Type

var adjustmentType: AVCaptionConversionAdjustment.AdjustmentType

The type of caption conversion adjustment.

struct AdjustmentType

Constants that indicate an adjustment type.

class AVCaptionConversionTimeRangeAdjustment

An object that describes an adjustment to the time range of one or more captions.

## Relationships

### Inherits From

- NSObject

### Inherited By

- AVCaptionConversionTimeRangeAdjustment

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Inspecting the Warning

var warningType: AVCaptionConversionWarning.WarningType

A type that indicates the nature of the validation warning.

var rangeOfCaptions: NSRange

The range of the captions for which the system issued a warning.

var adjustment: AVCaptionConversionAdjustment?

A correction the converter makes when it converts a caption to a specific format.

struct WarningType

The type of a caption conversion warning.

