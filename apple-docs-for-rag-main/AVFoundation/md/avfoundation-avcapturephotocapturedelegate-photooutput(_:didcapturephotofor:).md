

- AVFoundation
- AVCapturePhotoCaptureDelegate
-  photoOutput(\_:didCapturePhotoFor:) 

Instance Method

# photoOutput(\_:didCapturePhotoFor:)

Notifies the delegate that the photo has been taken.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
optional func photoOutput(
    _ output: AVCapturePhotoOutput,
    didCapturePhotoFor resolvedSettings: AVCaptureResolvedPhotoSettings
)
```

## Parameters 

`output`  

The photo output performing the capture.

`resolvedSettings`  

An object describing the settings used for this capture. Match this object’s uniqueID value to the uniqueID property of the photo settings object you initiated capture with to determine which capture request this delegate call corresponds to. You can also use this object to find out which values the photo output has chosen for automatic settings.

## Mentioned in 

Tracking Photo Capture Progress

## Discussion

The photo output calls this method as soon as the first step of capture ends—that is, at the end of the photographic exposure time.

## See Also

### Monitoring Capture Progress

func photoOutput(AVCapturePhotoOutput, willBeginCaptureFor: AVCaptureResolvedPhotoSettings)

Notifies the delegate that the capture output has resolved settings and will soon begin its capture process.

func photoOutput(AVCapturePhotoOutput, willCapturePhotoFor: AVCaptureResolvedPhotoSettings)

Notifies the delegate that photo capture is about to occur.

func photoOutput(AVCapturePhotoOutput, didFinishCaptureFor: AVCaptureResolvedPhotoSettings, error: (any Error)?)

Notifies the delegate that the capture process is complete.

