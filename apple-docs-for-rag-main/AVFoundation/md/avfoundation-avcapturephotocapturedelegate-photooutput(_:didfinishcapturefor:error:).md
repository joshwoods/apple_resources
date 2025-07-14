

- AVFoundation
- AVCapturePhotoCaptureDelegate
-  photoOutput(\_:didFinishCaptureFor:error:) 

Instance Method

# photoOutput(\_:didFinishCaptureFor:error:)

Notifies the delegate that the capture process is complete.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
optional func photoOutput(
    _ output: AVCapturePhotoOutput,
    didFinishCaptureFor resolvedSettings: AVCaptureResolvedPhotoSettings,
    error: (any Error)?
)
```

## Parameters 

`output`  

The photo output performing the capture.

`resolvedSettings`  

An object describing the settings used for this capture. Match this object’s uniqueID value to the uniqueID property of the photo settings object you initiated capture with to determine which capture request this delegate call corresponds to. You can also use this object to find out which values the photo output has chosen for automatic settings.

`error`  

If the capture process did not complete successfully, an error object describing the failure; otherwise, `nil`.

## Mentioned in 

Capturing Photos in RAW and Apple ProRAW Formats

Tracking Photo Capture Progress

## Discussion

The photo output calls this method when the entire capture process has finished, and no more delegate messages will be sent for this capture request. Use this time to clean up any resources you’ve allocated that relate to this capture request.

## See Also

### Monitoring Capture Progress

func photoOutput(AVCapturePhotoOutput, willBeginCaptureFor: AVCaptureResolvedPhotoSettings)

Notifies the delegate that the capture output has resolved settings and will soon begin its capture process.

func photoOutput(AVCapturePhotoOutput, willCapturePhotoFor: AVCaptureResolvedPhotoSettings)

Notifies the delegate that photo capture is about to occur.

func photoOutput(AVCapturePhotoOutput, didCapturePhotoFor: AVCaptureResolvedPhotoSettings)

Notifies the delegate that the photo has been taken.

