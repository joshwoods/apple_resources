

- AVFoundation
- AVCapturePhotoCaptureDelegate
-  photoOutput(\_:willCapturePhotoFor:) 

Instance Method

# photoOutput(\_:willCapturePhotoFor:)

Notifies the delegate that photo capture is about to occur.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
optional func photoOutput(
    _ output: AVCapturePhotoOutput,
    willCapturePhotoFor resolvedSettings: AVCaptureResolvedPhotoSettings
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

The photo output calls this method as close as possible to the initial moment of capture. If the shutter sound is enabled, this call occurs immediately after the photo output begins playing the shutter sound.

Note

Live Photo capture disables the shutter sound. In some regions, the device’s mute switch can disable the shutter sound.

## See Also

### Monitoring Capture Progress

func photoOutput(AVCapturePhotoOutput, willBeginCaptureFor: AVCaptureResolvedPhotoSettings)

Notifies the delegate that the capture output has resolved settings and will soon begin its capture process.

func photoOutput(AVCapturePhotoOutput, didCapturePhotoFor: AVCaptureResolvedPhotoSettings)

Notifies the delegate that the photo has been taken.

func photoOutput(AVCapturePhotoOutput, didFinishCaptureFor: AVCaptureResolvedPhotoSettings, error: (any Error)?)

Notifies the delegate that the capture process is complete.

