

- AVFoundation
- AVCapturePhoto
-  bracketSettings 

Instance Property

# bracketSettings

The variations available for bracketed capture settings for this photo.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var bracketSettings: AVCaptureBracketedStillImageSettings? { get }
```

## Discussion

When you request a bracketed capture using the AVCapturePhotoBracketSettings class, you specify an array of AVCaptureBracketedStillImageSettings objects indicating the capture setting variations (such as exposure compensation) to apply to each image in the bracket. This property indicates the settings associated with this particular photo, or `nil` if this photo is not part of a bracketed capture.

## See Also

### Examining Bracketed Capture Information

var sequenceCount: Int

The 1-based index of this photo in a bracketed capture sequence.

var lensStabilizationStatus: AVCaptureDevice.LensStabilizationStatus

Information about the use of lens stabilization during bracketed photo capture.

enum LensStabilizationStatus

Constants that indicate the status of optical image stabilization hardware during a bracketed photo capture.

