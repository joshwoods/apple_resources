

- AVFoundation
- AVCapturePhoto
-  sequenceCount 

Instance Property

# sequenceCount

The 1-based index of this photo in a bracketed capture sequence.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var sequenceCount: Int { get }
```

## Discussion

If this photo is part of a bracketed capture (requested with the AVCapturePhotoBracketSettings class), this property indicates the current result’s count in the sequence, starting with `1` for the first result.

If this photo is not part of a bracketed capture, this property’s value is `0`.

## See Also

### Examining Bracketed Capture Information

var bracketSettings: AVCaptureBracketedStillImageSettings?

The variations available for bracketed capture settings for this photo.

var lensStabilizationStatus: AVCaptureDevice.LensStabilizationStatus

Information about the use of lens stabilization during bracketed photo capture.

enum LensStabilizationStatus

Constants that indicate the status of optical image stabilization hardware during a bracketed photo capture.

