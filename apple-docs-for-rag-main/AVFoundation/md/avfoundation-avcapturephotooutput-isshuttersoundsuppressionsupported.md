

- AVFoundation
- AVCapturePhotoOutput
-  isShutterSoundSuppressionSupported 

Instance Property

# isShutterSoundSuppressionSupported

A Boolean value that indicates whether the photo output supports suppressing the system shutter sound.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
var isShutterSoundSuppressionSupported: Bool { get }
```

## Discussion

In iOS, the value is true, except in jurisdictions where you can’t disable the shutter sound. On all other platforms, the value is always false.

If the output supports this feature, you can supress the shutter sound when capturing a photo using the isShutterSoundSuppressionEnabled property of AVCapturePhotoSettings.

