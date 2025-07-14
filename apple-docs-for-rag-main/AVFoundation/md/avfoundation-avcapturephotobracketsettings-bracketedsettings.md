

- AVFoundation
- AVCapturePhotoBracketSettings
-  bracketedSettings 

Instance Property

# bracketedSettings

An array describing the number of and settings for images to produce in a bracketed capture.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var bracketedSettings: [AVCaptureBracketedStillImageSettings] { get }
```

## Discussion

This array is read-only. You provide this array of bracket settings when creating a settings object with the `init(format:rawPixelFormatType:bracketedSettings:)` initializer.

## See Also

### Working with Bracketed Settings

var isLensStabilizationEnabled: Bool

A Boolean value that specifies whether to stabilize the lens for the duration of the bracketed capture.

