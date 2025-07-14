

- AVFoundation
- AVCapturePhotoBracketSettings
-  isLensStabilizationEnabled 

Instance Property

# isLensStabilizationEnabled

A Boolean value that specifies whether to stabilize the lens for the duration of the bracketed capture.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var isLensStabilizationEnabled: Bool { get set }
```

## Mentioned in 

Capturing a Bracketed Photo Sequence

## Discussion

When this setting is true, the photo output uses optical image stabilization to hold the lens steady for the duration of the bracketed capture, helping to counter hand shake and produce a sharper bracket of images. The default setting is false.

You can enable this setting only if the photo output’s isLensStabilizationDuringBracketedCaptureSupported property is true. The capture output validates this requirement when you call the capturePhoto(with:delegate:) method. If your settings and delegate do not meet this requirement, that method raises an exception.

## See Also

### Working with Bracketed Settings

var bracketedSettings: [AVCaptureBracketedStillImageSettings]

An array describing the number of and settings for images to produce in a bracketed capture.

