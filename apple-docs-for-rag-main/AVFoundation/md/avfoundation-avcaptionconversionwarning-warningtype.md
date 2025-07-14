

- AVFoundation
- AVCaptionConversionWarning
-  warningType 

Instance Property

# warningType

A type that indicates the nature of the validation warning.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var warningType: AVCaptionConversionWarning.WarningType { get }
```

## See Also

### Inspecting the Warning

var rangeOfCaptions: NSRange

The range of the captions for which the system issued a warning.

var adjustment: AVCaptionConversionAdjustment?

A correction the converter makes when it converts a caption to a specific format.

class AVCaptionConversionAdjustment

An object that describes an adjustment to correct a problem found during validation of a caption conversion.

struct WarningType

The type of a caption conversion warning.

