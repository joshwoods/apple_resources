

- AVFoundation
- AVCapturePhotoCaptureDelegate
-  photoOutput(\_:willBeginCaptureFor:) 

Instance Method

# photoOutput(\_:willBeginCaptureFor:)

Notifies the delegate that the capture output has resolved settings and will soon begin its capture process.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
optional func photoOutput(
    _ output: AVCapturePhotoOutput,
    willBeginCaptureFor resolvedSettings: AVCaptureResolvedPhotoSettings
)
```

## Parameters 

`output`  

The photo output performing the capture.

`resolvedSettings`  

An object describing the settings used for this capture. Match this object’s uniqueID value to the uniqueID property of the photo settings object you initiated capture with to determine which capture request this delegate call corresponds to. You can also use this object to find out which values the photo output has chosen for automatic settings.

## Mentioned in 

Capturing and Saving Live Photos

Tracking Photo Capture Progress

## Discussion

The photo output calls this method when it has committed to a choice of settings and will soon begin the capture process. This call occurs as early as possible after your call to the capturePhoto(with:delegate:) method, letting you know what to expect for other delegate method calls related to the same capture.

Use this method and the AVCaptureResolvedPhotoSettings it provides to find out at the earliest possible opportunity which values the photo output has chosen for automatic settings, and what the output dimensions for captured images and movies will be. For example, if you requested capture with the flashMode property set to AVCaptureDevice.FlashMode.auto, the resolved photo settings’ isFlashEnabled property indicates whether the flash will fire during capture.

## See Also

### Monitoring Capture Progress

func photoOutput(AVCapturePhotoOutput, willCapturePhotoFor: AVCaptureResolvedPhotoSettings)

Notifies the delegate that photo capture is about to occur.

func photoOutput(AVCapturePhotoOutput, didCapturePhotoFor: AVCaptureResolvedPhotoSettings)

Notifies the delegate that the photo has been taken.

func photoOutput(AVCapturePhotoOutput, didFinishCaptureFor: AVCaptureResolvedPhotoSettings, error: (any Error)?)

Notifies the delegate that the capture process is complete.

