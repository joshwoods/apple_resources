

- AVFoundation
- AVCapturePhotoSettings
-  isShutterSoundSuppressionEnabled 

Instance Property

# isShutterSoundSuppressionEnabled

A Boolean value that indicates whether to suppress the built-in shutter sound when capturing a photo.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
var isShutterSoundSuppressionEnabled: Bool { get set }
```

## Discussion

The default value is false. Set the value to true to suppress the photo output’s built-in shutter sound for this request. The photo output throws an invalid argument exception when calling capturePhoto(with:delegate:) if its isShutterSoundSuppressionSupported property returns false.

