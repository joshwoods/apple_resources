

- AVFoundation
- AVCaptionConversionWarning
-  adjustment 

Instance Property

# adjustment

A correction the converter makes when it converts a caption to a specific format.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var adjustment: AVCaptionConversionAdjustment? { get }
```

## Discussion

If this value is `nil` and you perform the conversion without correcting the problem, the system doesn’t include captions that you indicate in the output media data.

## See Also

### Inspecting the Warning

var warningType: AVCaptionConversionWarning.WarningType

A type that indicates the nature of the validation warning.

var rangeOfCaptions: NSRange

The range of the captions for which the system issued a warning.

class AVCaptionConversionAdjustment

An object that describes an adjustment to correct a problem found during validation of a caption conversion.

struct WarningType

The type of a caption conversion warning.

