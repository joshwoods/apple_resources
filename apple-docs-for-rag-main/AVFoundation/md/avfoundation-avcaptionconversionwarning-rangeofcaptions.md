

- AVFoundation
- AVCaptionConversionWarning
-  rangeOfCaptions 

Instance Property

# rangeOfCaptions

The range of the captions for which the system issued a warning.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var rangeOfCaptions: NSRange { get }
```

## Discussion

This object only references captions with the same time range. If captions with different start times and durations have similar problems, or if individual captions have multiple problems, the validator generates separate instances of this class for each problem case.

## See Also

### Inspecting the Warning

var warningType: AVCaptionConversionWarning.WarningType

A type that indicates the nature of the validation warning.

var adjustment: AVCaptionConversionAdjustment?

A correction the converter makes when it converts a caption to a specific format.

class AVCaptionConversionAdjustment

An object that describes an adjustment to correct a problem found during validation of a caption conversion.

struct WarningType

The type of a caption conversion warning.

