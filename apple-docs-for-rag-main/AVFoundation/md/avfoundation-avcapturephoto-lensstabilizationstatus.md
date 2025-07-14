

- AVFoundation
- AVCapturePhoto
-  lensStabilizationStatus 

Instance Property

# lensStabilizationStatus

Information about the use of lens stabilization during bracketed photo capture.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var lensStabilizationStatus: AVCaptureDevice.LensStabilizationStatus { get }
```

## Discussion

This property applies only to capture results for which you requested optical image stabilization (OIS) across all frames of a bracketed photo capture (using the AVCapturePhotoBracketSettings isLensStabilizationEnabled property).

If the device configuration does not support OIS, this property’s value is AVCaptureDevice.LensStabilizationStatus.unsupported. If OIS is supported, but this captured photo is not from a bracketed capture where OIS was requested, this property’s value is AVCaptureDevice.LensStabilizationStatus.off. Otherwise, this property indicates how the device applied OIS across the duration of the bracketed capture.

## See Also

### Examining Bracketed Capture Information

var bracketSettings: AVCaptureBracketedStillImageSettings?

The variations available for bracketed capture settings for this photo.

var sequenceCount: Int

The 1-based index of this photo in a bracketed capture sequence.

enum LensStabilizationStatus

Constants that indicate the status of optical image stabilization hardware during a bracketed photo capture.

